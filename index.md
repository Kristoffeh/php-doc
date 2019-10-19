## Database Connection

```
<?php
$servername = "127.0.0.1"; // Database host
$username = ""; // Database username
$password = ""; // Password to db user
$db=""; // Name of database

// Establish connection
$conn = mysqli_connect($servername, $username, $password,$db);
?>
```

## Requirements

```
<?php
ob_start();
session_start();

require '../require/dbconnect.php';

$r=mysqli_query($conn, "SELECT * FROM users WHERE id='" . $_SESSION['id'] . "'");
$userRow=mysqli_fetch_array($r);

/*
if (!$query){
    printf("Error: %s\n", mysqli_error($conn));
    exit();
}*/
?>
```















## Welcome my page

You can use the [editor on GitHub](https://github.com/Kristoffeh/php-doc/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Kristoffeh/php-doc/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
