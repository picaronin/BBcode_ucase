# BBcode ucase
With this BBcode for phpBB the actual transformation of the selected text is achieved since Lowercase to Uppercase.

### BBCode usage:
```
[ucase]{TEXT}[/ucase]
```

### HTML replacement:
```
<span id="ucase1000">{TEXT}</span>
<script>
    var res = document.getElementById("ucase1000").innerHTML.toString().toUpperCase();
    var uniqid = Math.random().toString(36).replace(/[^a-z]+/g, '').substr(2, 10);
    document.getElementById("ucase1000").setAttribute("id", uniqid);
    document.getElementById(uniqid).innerHTML = res;
</script>
```

### Help line:
```
[ucase]TEXT[/ucase] Lowercase to Uppercase
```
