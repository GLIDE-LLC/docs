<br>

# Development Workflow

Complete project development workflow for **version control** of Glide projects.

This workflow deals with all stages of a project developmnt from start till launch. This workflow also includes process for properly supporting and maintaining the project after launch.

<br>

![alt text](images/1.png)

## 💯 WPEngine Site

Start off with the correct setup in WP engine website hosting account.

Guidelines on how to name these environments and their respective users is available here in [Glide Nomenclature](https://github.com/) document.

Make sure to follow the nomenclature guidelines in order to ensure same naming scheme across all projects and environments.

Following is the list of tasks to be performed on WP Engine.

<br>

1.  Add wp engine website `production environment`

2.  Add its `staging environment`

3.  Add its `development environment`

4.  Add one sftp user to each of these environments

5.  Open wordpress admin of `development environment`

6.  Update site title and tagline with project name

7.  Add admin user for Glide's use

8.  Add admin user for Client's use

9.  Copy `development environment` to both `staging` and `production environments`

<br>

***From this point onwards developers need to work in development environment only.***

More information on purpose of each WP Engine environment and how to use them can be found here in [WP Engine Environments](https://github.com/) document.

<br>

## 🌋 Local WP Site

Use [Local WP](https://github.com/) for setting up local WordPress environment.

Local WP is supported by WP Engine and it fully integrates with their service.

<br>

10. Open Local WP

11. Connect Local WP with WP Engine Account

12. Pull `development environment` of your project into Local WP

<br>

If for any reason you can not pull the `development environment`, add a new site to Local WP.

Make sure to follow the Glide [naming scheme](https://github.com/) for this purpose.

<br>

## 💯 Local Repository

<br>

13. Open Local WP project folder and convert it into a local repository

14. Add .gitignore file

15. Add base theme to themes folder

<br>

## Github Repository

16. Create repository in github

17. Connect local and github repositories

18. Add action in github for continuous deployment

19. Connect WP Engine development environment and github

20. Update base theme with project name

21. Stage, commit and push the first change in master branch

<br>

## Github Branches
---

22. Create development branch from master branch

23. Create developer branches from development branch

24. Merge developer branches back into developmeant branch

25. Create release branch from development branch

26. Update version number in theme files and test code

---
## First Release - v1.0.0
---

27. Merge release branch into master branch

28. Automatic deployment pushes code to development environment on wp engine

29. Tag master branch with new version number

30. Merge release branch back into development branch

31. Push database from Local WP to WP Engine

32. Review development environment

33. Copy development environment to staging environment

34. Share staging environment with reviewers

---
## Reviews & Tickets
---

35. Create developer branches from development branch

36. Pull latest version of database (if required.

37. Pull latest version of uploads folder (if required.

38. Merge developer branches back into developmeant branch

---
## Second Release v1.0.1
---

39. Create release branch from development branch

40. Update version number in theme files and test code

41. Merge release branch into master branch

42. Automatic deployment pushes code to development environment on wp engine

43. Tag master branch with new version number

44. Merge release branch back into development branch

45. Review development environment

46. Copy development environment to staging environment (files only.

47. Do content and image edits on staging environment (if required.

48. Share staging environment with reviewers

49. On approval copy staging environment down to development environment

---
## Launch Release v2.0.0
---

50. Create release branch from development branch

51. Update version number in theme files and test code

52. Merge release branch into master branch

53. Automatic deployment pushes code to development environment on wp engine

54. Tag master branch with new version number

55. Merge release branch back into development branch

56. Review development environment

57. Copy development environment to staging environment (files only.

58. Do content and image edits on staging environment (if required.

59. Share staging environment with reviewers

60. On approval copy staging environment down to development environment

---
## Launch
---

61. Copy approved staging environment to production environment

---
## Support
---

62. Copy production environment to staging environment

63. Copy staging environment to development environment

64. Create developer branch from development branch

65. Pull latest version of database to Local WP (if required.

66. Pull latest version of uploads folder to Local WP (if required.

67. Merge developer branches back into development branch

---
## Support Release v2.0.1
---

68. Create release branch from development branch

69. Update version number in theme files and test code

70. Merge release branch into master branch

71. Automatic deployment pushes code to development environment on wp engine

72. Tag master branch with new version number

73. Merge release branch back into development branch

74. Review development environment

75. Copy development environment to staging environment (files only.

76. Do content and image edits on staging environment (if required.

77. Share staging environment with reviewers

78. On approval copy staging environment down to development environment

79. Copy approved staging environment to production environment
