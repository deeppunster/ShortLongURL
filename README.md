# ShortLongURL
Create short strings to substitute for a long URL.

## Program Comments

*   Lots of comments added so our less experienced folks can
    hopefully follow the program flow and understand the steps taken.

*   The problem statement was taken as solving a small part of a
    much larger project.  As a result several assumptions were made:

    *   Permanent storage (e.g. to disk or cloud) would be
        handled later.
    *   Efficiencies of storage would be addressed later.
    *   How fast it ran was not yet a concern.

*   Using a class to manage the history is an example of
    encapsulating the details so the code outside of the class
    does not know or care about the reesults are derived.

*   Testing this solution is incomplete since it does not check the
    "edge" cases.  Full testing would include:

    *   Original URL is empty string or null
    *   Short string is empty or null
    *   Full URL fed to restore method
    *   Short string fed to shorten method
    *   Non-URLs for original URL (numbers, no prefix, etc.)


## For the more experienced developers

Yes, this solution has far more comments and methods than would be
written in production programs.  Perhaps in production it would be
reduced from a class to two functions.

The testing done under main would be managed by pytest in production
(or perhaps using BDD).  Since the focus of the problem is getting a
"first pass" solution, this testing is considered sufficient.
