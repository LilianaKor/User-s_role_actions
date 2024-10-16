# User-s_role_actions
To achieve a similar structure in Python for testing multiple user roles in an automation test framework (e.g., using pytest and selenium), you can follow a data-driven approach. Here's how you can write reusable functions for login, action, and logout, and loop through different user roles.

Key Points of the Code:
Reusable Functions: The perform_test() function handles login, performing role-based actions, and logout.
Data-Driven Testing: The users array contains different user credentials and roles. Instead of writing individual tests for each user role, we loop through them.
Parametrization: Using pytest's @pytest.mark.parametrize decorator, the same test logic is applied dynamically to different user roles.
Role-Based Actions: Based on the user's role, the appropriate actions are performed in the test.
Explanation of Test Optimization:
✅ Reusable Code: You’ve created a single reusable function that handles login, actions, and logout, making the test suite cleaner and more maintainable.
🔁 Dynamic Test Execution: Instead of creating multiple tests for each user role, the test logic runs dynamically for all scenarios, reducing redundancy.
📊 Data-Driven Testing: This approach allows you to run the same test logic for different data sets (e.g., different users and roles), enhancing test coverage while maintaining a compact codebase.
By organizing your tests this way, you make your test suite more efficient and reduce duplication. You only need to update the user data array if roles change, rather than modifying multiple test cases.

🎉 Outcome: This method significantly reduces the amount of test code while ensuring each user role is thoroughly tested!
