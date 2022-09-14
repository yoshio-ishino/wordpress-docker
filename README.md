# wordpress for development

## How to use REST-API without SSL.

* set `wp_is_application_Passwords_available` true
```
function wp_is_application_passwords_available() {
	/**
	 * Filters whether Application Passwords is available.
	 *
	 * @since 5.6.0
	 *
	 * @param bool $available True if available, false otherwise.
	 */
	return apply_filters( 'wp_is_application_passwords_available', '__return_true' );
}
```
