**

## Notes about Fly.io hiring app

**

**General notes**
I had some issues when trying to deploy the phoenix application using `flyctl deploy`.
I was getting the following error:

==> Creating release

    Error Deploying over the remote builder is not allowed.

After doing some research, I found that using `flyctl apps destroy` to destroy the app and creating it again sometimes worked to fix these kind of issues. In my case it worked and I was able to continue deploying and testing the different fly commands.

**What you built and what you didn't build**
I believe I built all the things that were in the project specification:

 - Added the data from the output of the fly status command to the dashboard
 - Refresh the data every few seconds
 - Deployed the application to the fly platform

**What you'd improve or fix if you had more time**
- Refactor the show template to avoid having one big file with lots of nested tags

**How you'd determine if this feature is successful**
If I can get the expected output every time I deploy the application and every time the page is refreshed, then I can think the feature was successful. Usually when there is time to do tests, also doing these tests is a very good way to determine the feature is successful. And third, another important point to take into consideration is the feedback from end users.