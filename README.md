# Social Login with Spring Boot 2.0
 
This example app shows how to add social login to a Spring Boot app with Okta.

Please read [Add Social Login to Your Spring Boot 2.0 App](https://developer.okta.com/blog/2018/07/24/social-spring-boot) to see how this app was created.

**Prerequisites:** [Java 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) and an [Okta Developer Account](https://developer.okta.com).

> [Okta](https://developer.okta.com/) has Authentication and User Management APIs that reduce development time with instant-on, scalable user infrastructure. Okta's intuitive API and expert support make it easy for developers to authenticate, manage, and secure users and roles in any application.

* [Getting Started](#getting-started)
* [Links](#links)
* [Help](#help)
* [License](#license)

## Getting Started

You will need to create an OIDC Application in Okta to get your settings to perform authentication. 

1. Log in to your developer account on [developer.okta.com](https://developer.okta.com).
2. Navigate to **Applications** and click on **Add Application**.
3. Select **Web** and click **Next**. 
4. Give the application a name, add `http://localhost:8080/authorization-code/callback` as a Login redirect URI, and click **Done**.
5. Edit the project and enable "Implicit (Hybrid)" as a grant type and click **Save**.

Copy `src/main/resources/application.template.yml` to `src/main/resources/application.yml` and fill in the necessary information.

See [these instructions](https://developer.okta.com/blog/2018/07/24/social-spring-boot#configure-google-and-facebook-for-social-login-in-your-spring-boot-app) to complete your social login setup.

## Links

This example uses the following open source libraries:

* [Okta Sign-In Widget](https://github.com/okta/okta-signin-widget)
* [Okta Spring Boot Starter](https://github.com/okta/okta-spring-boot)
* [Spring Boot](https://spring.io/projects/spring-boot)
* [Spring Security](https://spring.io/projects/spring-security)

## Help

Please post any questions as comments on the [blog post](https://developer.okta.com/blog/2018/07/24/social-spring-boot), or visit our [Okta Developer Forums](https://devforum.okta.com/). You can also email developers@okta.com if you'd like to create a support ticket.

## License

Apache 2.0, see [LICENSE](LICENSE).
