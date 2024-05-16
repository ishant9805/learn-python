# Advanced Python

## Virtual Environments

Question: What is a Virtual Environment?

Answer: A virtual environment is a tool which lets a deveolper create an isolated Python environment. 

Question: What is the need of Virtual Environments?

Answer: It helps in isolation of packages you are using in a python project. Consequently, resolving the conflicts of version of libraries in different projects.


Let us understand it with a scenario.
--
**Scenario**: Ishant is a developer who is currently working on a Django project and he is starting this project. So, he just installed latest version of Django (Django 5.0.6) and started working on it. After working on that project from sometime, He just got a freelance project where he needs to develop a feature using Django. But the project was started a year ago and at that time Django 4.2.2 was released.

**Solution 1**: He can uninstall the latest Django version from system and install Django 4.2.2. But this solution won't help him as whenever he switches between the projects he need to uninstall and reinstall different versions of Django again and again which will be tedious. 

**Solution 2**: If he directly installs Django 4.2.2. Either he will be facing issues related to version confliction or he will face errors while installing the package.

**Solution 3**: He can use virtual environments to resolve the issue. He can create a virtual python environment for his own project where he will install Django 5.0.6 and create a separate environment for his client's project and install Django 4.2.2 there. Then there will be no conflicts while development.

The following infographic might help you.

![Image](xyz)

---
What happens behind the scene?
When you create virtual environment, it creates a directory which contains configs, scripts and a link to python interpreter. Now, whenever you install a python package while being in that environment, the packages will be installed in that same directory isolating from system wide installed packages and packages of other project.