Individual-HW4
HW4 - Staff Role Functionality Extension

This repository is part of CSE360 HW4, where additional user stories related to the Staff role have been implemented based on the TP3 project. This version introduces new capabilities for staff users such as deleting reviews, managing user roles, viewing all users, and accessing flagged content.

 Project Structure

All relevant code is located in:
IndividualHW.zip file, which you can download from Github


Key Java files for this assignment:

- StaffHomePage.java – JavaFX GUI for staff role features
- ReviewManager.java – Business logic and data access interface
- DatabaseHelper.java – Contains all SQL operations for user, review, and moderation features
- Review.java` and `User.java – Data model classes used throughout the app

 Implemented Staff User Stories

1. Delete reviews by ID  
   - UI in `StaffHomePage.java`
   - Logic in `ReviewManager.deleteReviewById(int reviewId)`
   - Uses `DatabaseHelper.deleteReview(reviewId)`

2. View all users  
   - `StaffHomePage.java` fetches users using `ReviewManager.getAllUsers()`

3. Change a user's role
   - Uses `ReviewManager.updateUserRole(int userId, String newRole)` which internally calls `DatabaseHelper.updateUserRole(...)`

4. View flagged reviews
   - Staff can see flagged content using `ReviewManager.getFlaggedReviews()` from the database

 Unit Tests (JUnit)

Unit test file:  
I will make a folder and upload the Test code in that 

Javadoc:
A seperate Javadoc folder has been made for you to take a look at the PDF 
