laravel-l18n-generator
======================

Laravel-l18n-generator is a tool that allow you to generate the l10n file from the source file. 

Place the "data-lzn" attribute on a html/blade tag, run the generator, and the text into the tag is replace by the "__" laravel helper.

Before : 

```
...
<p data-lzn>Hello world guys!</p>
...
```
Run:

```
$ l10n-gen .
```
After:

```
...
  <p>__('index_blade_html_89')</p>
...  
```

And within the application/language/en/l10n-generator.php file :

```
return array(
     'index_blade_html_89' => 'Hello world guys!',
);
```
