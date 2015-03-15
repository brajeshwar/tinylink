# Tiny Link #

This wordpress plugin creates an alternate TinyURL link to your article or post permalink. This will be useful while giving out links while sending emails, mobile devices, et al.

## README ##

### INSTALL ###

  * [Download](http://code.google.com/p/tinylink/downloads/list) the plugin
  * Active the pugin through your Wordpress Admin > Plugins

### USAGE ###

**SIMPLE**

Just use `<?php TinyLink() ?>` wherever you wish the link to appear.

**ADVANCE**

Here, we check if the plugin is installed, if yes, then execute this section. We can even give a direct link to it, so users can copy the link by right-clicking (Mac: Ctrl+Left Click) the hyperlink.

```
<?php if (function_exists('TinyLink')) { ?>
Tiny alternate link for this article: 
<a href="<?php TinyLink() ?>" title="TinyURL link to - <?php the_title(); ?>"><?php TinyLink() ?></a>
<?php } ?>
```