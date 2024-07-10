## A start component

start Component with: 

- entities
- data
- services
- REST API
- screens

To install run (with moqui-framework):

```bash
# In Moqui Framework Directory
export NEW_COMPONENT_NAME=new
cd runtime/component
git clone https://github.com/acetousk/start
cd start
find . -type f -exec sed -i "s/start/${NEW_COMPONENT_NAME}/g" {} +
cd ..
mv start ${NEW_COMPONENT_NAME}
```
