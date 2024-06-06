# How to Contribute to Docs

## **Website Documentation Guidelines**
If you haven't build website locally yet, run following commands inside `theupdateframework` directory (use your [forked](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://docs.github.com/articles/fork-a-repo&ved=2ahUKEwjexbXp6aqGAxXP1zgGHYMfB3AQFnoECAkQAQ&usg=AOvVaw3knkDqfZXHdtlZVtWiPqst) repository)
```
 $ yarn install
 $ hugo server
```
This will run website locally on http://localhost:1313 by default. 

The [content](https://github.com/theupdateframework/theupdateframework.io/tree/master/content) directory is used as a source for Markdown files (Docs), which Hugo uses to generate the TUF website resources.

### **Add Menu on Website**
___

The starting step is to add a route to render your Markdown file.

Navigate to the [config.toml](https://github.com/theupdateframework/theupdateframework.io/blob/master/config.toml) file.

### **Create Menu with Submenu options**
When the Menu contains SubMenu options:

- Use the following format:
```toml
[[menu.main]]
name = "<Menu>"
identifier ="<Menu_Identifier>"
weight = <order>
```
- Place the Menu at the relevent position in [config.toml](https://github.com/theupdateframework/theupdateframework.io/blob/master/config.toml) based on its weight.
- Restart the Hugo server to see changes.

### **Create Menu without SubMenu options**

When the Menu does not contain any Submenu options:

- Use the following format:
```toml
[[menu.main]]
name = "<Menu>"
url = "/<route>/"
weight = <order>
```

- Place the section at the relevant position according to its weight in [config.toml](https://github.com/theupdateframework/theupdateframework.io/blob/master/config.toml).
- Restart the Hugo server, to see changes.

### **Add SubMenu options to Parent Menu**
___

- Use the following format:
```toml
[[menu.main]]
name = "<SubMenu_Heading>"
parent = "<Menu>"
url = "/<route>"  #This should be in lowercase, relates to SubMenu heading, and should not conflict with other routes
weight = <order>
```

- Position the SubMenu at the relevant place according to its weight in [config.toml](https://github.com/theupdateframework/theupdateframework.io/blob/master/config.toml).
- Restart the Hugo server, to see changes.



### **Markdown Files for Menu or SubMenu options**
___

- The Markdown file name should be `<route>.md` for consistency.
- Front Matter is essential on top of every Markdown. In Hugo, the title is defined like this:
```markdown
---
title: <title>
---
```
else file content can be written according to [Markdown rules](https://www.markdownguide.org/basic-syntax/) and [Hugo Markdown Support](https://www.markdownguide.org/tools/hugo/#hugo-markdown-support). 

### Need Help?
If you feel any doubt or issue, Please feel free to [Join us](https://github.com/theupdateframework/community?tab=readme-ov-file#tuf-community)
