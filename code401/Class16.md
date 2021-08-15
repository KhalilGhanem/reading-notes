# Spring Authentication

## Authentication and Access Control
Application security boils down to two more or less independent problems: authentication (who are you?) and authorization (what are you allowed to do?) Sometimes people say “access control” instead of "authorization".

### Authentication
The main strategy interface for authentication is AuthenticationManager, which has only one method the authenticate() method:
```
public interface AuthenticationManager {

  Authentication authenticate(Authentication authentication)
    throws AuthenticationException;
}
```
which can do :
* Return an Authentication (normally with authenticated=true) if it can verify that the input represents a valid principal.
* Throw an AuthenticationException if it believes that the input represents an invalid principal.

   * AuthenticationException is a runtime exception. It is usually handled by an application in a generic way, depending on the style or purpose of the application.

* Return null if it cannot decide.


AuthenticationProvider is a bit like an AuthenticationManager, but it has an extra method to allow the caller to query whether it supports a given Authentication type:
```
public interface AuthenticationProvider {

	Authentication authenticate(Authentication authentication)
			throws AuthenticationException;

	boolean supports(Class<?> authentication);
}
```

## Authorization or Access Control
Once authentication is successful, we can move on to authorization, and the core strategy here is AccessDecisionManager. There are three implementations provided by the framework and all three delegate to a chain of AccessDecisionVoter instances, a bit like the ProviderManager delegates to AuthenticationProviders.

An AccessDecisionVoter considers an Authentication (representing a principal) and a secure Object, which has been decorated with ConfigAttributes:
```
boolean supports(ConfigAttribute attribute);

boolean supports(Class<?> clazz);

int vote(Authentication authentication, S object,
        Collection<ConfigAttribute> attributes);
```