## A start component

start Component with: 

- entities
- data
- services
- REST API
- screens

Create a new git repository at ${NEW_COMPONENT_NAME}

To install and push to your new repo run (with moqui-framework):

```bash
# In Moqui Framework Directory
export NEW_COMPONENT_NAME=new # Change this to something else
export GIT_USERNAME=me # Change this to something else
cd runtime/component
git clone https://github.com/acetousk/start
cd start
find . -type f -exec sed -i "s/start/${NEW_COMPONENT_NAME}/g" {} +
git remote set-url origin git@github.com:${GIT_USERNAME}/${NEW_COMPONENT_NAME}
git branch -M master
git push -u origin master
cd ..
mv start ${NEW_COMPONENT_NAME}
cd ../..
```
