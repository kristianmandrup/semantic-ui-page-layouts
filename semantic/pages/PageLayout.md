```html
<!-- after sidebar -->
<div class="ui black big launch right attached fixed button">
  <i class="content icon"></i>
  <span class="text">Menu</span>
</div>

<!-- main menu -->
<div class="ui fixed inverted main menu">
  <div class="ui container">
    <a class="launch icon item">
      <i class="content icon"></i>
    </a>
```

Try this:

https://github.com/Semantic-Org/Semantic-UI/issues/945

http://stackoverflow.com/questions/21910566/attach-button-to-semantic-ui-sidebar

Use the 'exclusive' setting to display multiple sidebars that play nicely with each other.

`$('.your-shared-sidebar-class').sidebar('setting','exclusive',false).sidebar('show');`

```html
<script language="javascript" src="http://code.jquery.com/jquery.min.js"></script>
<script language="javascript" src="[your path here]/semantic.js"></script>

<script type="text/javascript">

    $(document).ready(function() {
        $('.left.demo.sidebar').sidebar('toggle');
    });

</script>
```
