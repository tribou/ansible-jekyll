ansible-jekyll
=============

Install simple nginx instance with a Jekyll build off a bare git repo.
[Credit goes out to this awesome blog post](https://www.digitalocean.com/community/tutorials/how-to-deploy-jekyll-blogs-with-git)

#### Execute

First, copy the group_vars/jekyll.yml to a local group_vars/jekyll.yml file and customize the variables to your needs.

```bash
ansible-playbook site.yml
```

Use a private key if needed.

Then, to deploy a Jekyll site to your new server:

```bash
git remote add prod git@example.org:repos/example-repo.git
git push prod master
```
