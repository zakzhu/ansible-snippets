1. command line values (eg “-u user”)
2. **role defaults**
3. inventory file or script group vars
4. inventory group_vars/all
5. playbook group_vars/all
6. inventory group_vars/\*
7. playbook group_vars/\*
8. inventory file or script host vars
9. inventory host_vars/\*
10. playbook host_vars/\*
11. host facts / cached set_facts
12. play vars
13. play vars_prompt
14. play vars_files
15. role vars (defined in role/vars/main.yml)
16. block vars (only for tasks in block)
17. task vars (only for the task)
18. include_vars
19. set_facts / registered vars
20. role (and include_role) params
21. include params
22. extra vars (always win precedence, eg "-e name=zak")
