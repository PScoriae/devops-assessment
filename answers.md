1. A fast-growing application requires multiple teams working together with high
   velocity and less dependency on each other during development. For example, User
   Profile is a shared resource throughout the application and any changes might break
   a feature. Propose a one-page solution with plans and technology stack you might
   use to reduce breaking changes and dependencies.
   (10 points)

First, Source Control Management (SCM) for repository code should be used. With Git's version control and the use of a distributed cloud version control service such as GitHub or GitLab, the origin server, software developers can first commit their changes locally and then push it to the origin repository in the cloud for other developers to pull. Through the use of Git branches, each developer can branch off from the main branch to work on their respective feature or bugfix so as to prevent any conflicts with other developers' changes in code.

Of course, while Git itself is a great tool for developers to manage and organise the codebase, it's also important to note the best practices on how to use it as well as the proper communication required to prevent merge conflicts and breaking changes.

One practice that all developers should habitualise is to frequently commit changes and push them to the origin server as well as frequently pulling from the origin server. This is one of the ways breaking changes can be prevented since frequent small commits are less likely to have huge sudden changes in the code that may affect each developer's local code.

Communication is also vital between developers. For example, picture two developers working on two different branches, Branch B and Branch C, that branch out from the same branch, Branch A. There's a bug in Branch A, so both developers make changes to the same lines of code in their own branches albeit with different approaches. If they both try to merge their changes back into Branch A, there will be a merge conflict. While this is the proper use of branches, the problem here is the lack of communication between developers, something rather vital when it comes to DevOps and Agile based teams. If both developers had known each others tasks, they wouldn't have had this merge conflict to deal with.

Second,

As for the plans and technology stack to be used for this team, Git should be used as the version control system with GitHub as the distributed cloud-based origin git repository.

2. Significant changes are much easier to develop on a new application than on an
   existing one. The challenge is to migrate existing data to the new application. The
   easiest solution is to have downtime, but how would you do it without downtime?
   Propose a two-page solution with plans and technology stack you would use for the
   migration with less impact on the user experience.
   (20 points)

3. Deploying a new feature for an application can be a hassle if something unexpected
   happens. To control the feature rollout, it's best to have multiple stages of
   deployment that can be rolled back. For example, the first deployment only affects
   users in Malaysia before the second deployment affects users throughout Southeast
   Asia. the users won’t feel any changes if the rollback happens. Propose a two-page solution with plans and technology stack to achieve a smooth transition during the
   deployment rollout and rollback.
   (20 points)
