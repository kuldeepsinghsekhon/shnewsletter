step 1: Upload all images, css and js files to assets in template editor.Make sure you are uploading images and .js files only.Remaining files to copy in next steps

step 2: Open newsletter-popup.liquid and copy all code.Now in Snippets click on "Add a New Snippet".Name it "newsletter-popup.liquid" and paste all code of newsletter-popup.liquid.

step 3: Same once again. Open newsletter.liquid and copy all code.Now in Snippets click on "Add a New Snippet".Name it "newsletter-popup.liquid" and paste all code of newsletter.liquid.

step 4:open theme settings code file, copy and paste it to last config > settings.html 

step 5:Now open "theme.liquid" file and paste it in header 

{{ 'jquery-1.7.min.js' | asset_url | script_tag }}
{{ 'fancy.js' | asset_url | script_tag }}


step 6 in the "theme.liquid" file, Go to end of file.
add this line just befor end of body tag like this.

{% include 'newsletter-popup' %}
</body>
