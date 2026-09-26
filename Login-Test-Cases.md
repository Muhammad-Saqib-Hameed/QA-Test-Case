TC ID	Test Scenario	Test Steps	Expected Result	Priority
TC_LOGIN_001	Login with valid credentials	Enter valid email and valid password → Click Login	User should be logged in successfully and redirected to the dashboard/home page	High
TC_LOGIN_002	Login with valid email and invalid password	Enter valid email → Enter incorrect password → Click Login	Appropriate error message should be displayed and user should not be logged in	High
TC_LOGIN_003	Login with invalid email and valid password	Enter unregistered email → Enter valid password → Click Login	Login should fail and an appropriate error message should be displayed	High
TC_LOGIN_004	Login with invalid email and invalid password	Enter invalid email → Enter invalid password → Click Login	Login should fail without exposing sensitive information	High
TC_LOGIN_005	Login with both fields empty	Leave email and password empty → Click Login	Required-field validation messages should be displayed	High
TC_LOGIN_006	Login with empty email	Leave email empty → Enter valid password → Click Login	Email required-field validation should be displayed	High
TC_LOGIN_007	Login with empty password	Enter valid email → Leave password empty → Click Login	Password required-field validation should be displayed	High
TC_LOGIN_008	Enter invalid email format	Enter test@ → Enter valid password → Click Login	Email format validation should be displayed	Medium
TC_LOGIN_009	Enter email without @ symbol	Enter testexample.com → Enter password → Click Login	Invalid email format message should be displayed	Medium
TC_LOGIN_010	Enter email without domain	Enter test@example → Enter password → Click Login	Invalid email format message should be displayed	Medium
TC_LOGIN_011	Verify password masking	Enter password in password field	Password characters should be masked/hidden	Medium
TC_LOGIN_012	Verify password visibility toggle	Enter password → Click the eye/show-password icon	Password should become visible; clicking again should mask it	Medium
TC_LOGIN_013	Verify email field accepts valid email	Enter a valid email address	Email should be accepted without validation error	Medium
TC_LOGIN_014	Verify password field accepts valid password	Enter a valid password	Password should be accepted according to defined password rules	Medium
TC_LOGIN_015	Verify email field maximum length	Enter an email exceeding the allowed length	Application should prevent excessive input or display appropriate validation	Medium
TC_LOGIN_016	Verify password maximum length	Enter a password exceeding the allowed length	Application should handle the input according to defined requirements	Medium
TC_LOGIN_017	Enter leading/trailing spaces in email	Enter test@example.com → Enter valid password → Login	Application should handle surrounding spaces according to requirements, normally by trimming them	Medium
TC_LOGIN_018	Enter spaces only in email	Enter only spaces in email → Enter password → Login	Email validation should be displayed and login should fail	Medium
TC_LOGIN_019	Enter spaces only in password	Enter valid email → Enter only spaces in password → Login	Password validation should be displayed and login should fail	Medium
TC_LOGIN_020	Press Enter to submit login	Enter valid credentials → Press Enter	Login should be submitted successfully	Medium
TC_LOGIN_021	Verify Login button state	Open login page without entering credentials	Login button should behave according to the application's validation/design requirements	Low
TC_LOGIN_022	Verify error message for failed login	Enter incorrect credentials	Clear and appropriate error message should be displayed	High
TC_LOGIN_023	Verify error message disappears after correction	Enter invalid credentials → Receive error → Correct credentials	Previous error should disappear or update appropriately	Medium
TC_LOGIN_024	Verify successful login redirect	Enter valid credentials → Click Login	User should be redirected to the correct authenticated page	High
TC_LOGIN_025	Verify session after successful login	Login successfully → Navigate to another authenticated page	User should remain authenticated during the valid session	High
TC_LOGIN_026	Access protected page without login	Log out → Try to access a protected URL directly	User should be redirected to the login page or denied access	High
TC_LOGIN_027	Verify logout	Login successfully → Click Logout	User should be logged out and redirected appropriately	High
TC_LOGIN_028	Browser Back button after logout	Login → Logout → Press browser Back	User should not regain access to protected content	High
TC_LOGIN_029	Refresh page after successful login	Login successfully → Refresh the page	User should remain logged in if the session is still valid	Medium
TC_LOGIN_030	Refresh login page	Open login page → Enter data → Refresh page	Application should handle entered credentials according to security requirements; password should not be exposed or improperly retained	High
TC_LOGIN_031	Verify Forgot Password link	Click Forgot Password	User should be redirected to the password recovery page	High
TC_LOGIN_032	Forgot Password with registered email	Open Forgot Password → Enter registered email → Submit	Password recovery process should start successfully	High
TC_LOGIN_033	Forgot Password with unregistered email	Enter an unregistered email → Submit	Application should display an appropriate response without unnecessarily revealing whether an account exists	High
TC_LOGIN_034	Verify Remember Me option	Select Remember Me → Login → Close/reopen browser	User session should behave according to the Remember Me requirements	Medium
TC_LOGIN_035	Verify login page on mobile screen	Open login page on a mobile-sized viewport	Login form should be responsive and usable without layout issues	Medium
TC_LOGIN_036	Verify login page on different browsers	Test login on Chrome, Edge, Firefox, etc.	Login functionality and UI should work consistently across supported browsers	Medium
TC_LOGIN_037	Verify keyboard navigation	Use Tab/Shift+Tab to navigate through login controls	Focus should move logically through the fields and controls	Medium
TC_LOGIN_038	Verify focus on email field	Open login page	Cursor/focus should be placed according to the UI requirements	Low
TC_LOGIN_039	Verify login button during multiple clicks	Enter valid credentials → Quickly click Login multiple times	Application should prevent duplicate login requests or handle them safely	High
TC_LOGIN_040	Verify login with special characters	Enter valid credentials containing supported special characters → Login	Application should correctly handle valid special characters without errors	Medium
TC_LOGIN_041	Verify case handling for email	Enter email with different letter casing → Enter valid password	Email handling should follow the application's defined case-sensitivity rules	Medium
TC_LOGIN_042	Verify password case sensitivity	Enter correct email → Change password letter casing → Login	Login should fail if the password is case-sensitive	High
TC_LOGIN_043	Verify account lockout/rate limiting	Enter incorrect password repeatedly according to the application's security policy	Account/request should be handled according to configured lockout or rate-limit rules	High
TC_LOGIN_044	Verify SQL injection input	Enter a SQL injection-style string in the email/password fields	Application should reject/handle the input safely without exposing database information	Critical
TC_LOGIN_045	Verify XSS input	Enter a script-like payload into login fields	Input should be safely handled and no script should execute	Critical
TC_LOGIN_046	Verify password is not exposed in URL	Submit login credentials	Password should never appear in the URL	Critical
TC_LOGIN_047	Verify HTTPS	Open login page and inspect browser connection	Login page and credential submission should use HTTPS	Critical
TC_LOGIN_048	Verify password is not stored in browser autocomplete if prohibited	Inspect password field behavior	Password handling should follow the application's security requirements	High
TC_LOGIN_049	Verify session timeout	Login successfully → Remain inactive until configured session timeout	User should be logged out or asked to authenticate again according to session policy	High
TC_LOGIN_050	Verify concurrent login sessions	Login from multiple supported devices/browsers	Behavior should match the application's session-management requirements	Medium
| Status | Not Executed |
