Reviews of the code

The code uses Eloquent and Repository pattern techniques instead of using Query Builder which is a good way to optimize as well as Centralization of the data access logic makes the code easier to maintain.
The only above point makes it good but not amazing because if the controller and repository naming convention belong to the Bookings then it should consist of the code for the bookings data not for the Job data (should be terrible).

Now if we consider the same code for further evaluation then:

1. The code has format and structure but needs to be shorter and readable by removing unnecessary code lines.
2. Mass assignment in the code! which is very terrible however you have an eloquent and $request->all() approach.
3. Never should access the env variable directly, try to use config based.
4. The code comments are not descriptive according to standards.
5. If considering the logically wise then the code does not fulfill the "Single responsibility principle" and the "DRY" approach is too bad, lengthy, and non-efficient.

I might be wrong but according to my experience, I observed the above points and mentioned the reviews.

Further, If we proceed to refactor the code then it must fulfill the correct naming convention but I am eliminating this and will modify only existing code in the existing files to save time.
