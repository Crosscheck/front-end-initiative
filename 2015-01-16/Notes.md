# Front end initiative 2015-01-16
## Notes
  
### boilerplate
  * 3 [releases](https://github.com/Crosscheck/drupal-theme-boilerplate/releases)
  * new [issues](https://github.com/Crosscheck/drupal-theme-boilerplate/issues) 19 total

### Scsslinting
  * Project scss health
  * Everyone on the team is enforced to code in the same way
  * [scss-lint](https://github.com/causes/scss-lint) is a Ruby gem
  * grunt configuration [options](https://github.com/ahmednuaman/grunt-scss-lint)
  * see [option](https://github.com/causes/scss-lint/blob/master/lib/scss_lint/linter/README.md) list
  * file per file configuration with exclude: & include:
      
        options:
          bundleExec: true
          config: "scsslint.yml"
          colorizeOutput: true
        allFiles: [
          "<%= settings.base %><%= settings.theme %>assets/scss/**/*.scss"
        ]

### Theme file spec

  * For template debugging
  * should only be enabled on dev
  * theme developer
  * drupal 8 twig debug

    <?php if( theme_get_setting('themer_helper') ) : ?>
      <?php print __FILE__; ?>
    <?php endif; ?>

### Sourcemaps
  * since sass 3.3 sourcemaps support
  * Inspect scss files in dev mode
  * setup in [browsers](http://thesassway.com/intermediate/using-source-maps-with-sass)


### Sass 3.4.x
  * [changelog](http://sass-lang.com/documentation/file.SASS_CHANGELOG.html)


### layout rules split up
  * advantages
    * mediaqueries based on pages
    * separation of global layout and page layout
    * mediaqueries of components can still  in components
    * [structure](https://dl.dropboxusercontent.com/u/7422112/screenshots/Screen%20Shot%202015-01-16%20at%2010.48.12.png)
    * example:

```css

      .node--gemeentelijk-adres--full {
        .contact {
          margin-bottom: 20px;
          @include box-sizing(border-box);
          @include typo($body_font_family, $font_size, $font_size, $white);
          padding: 25px;

          h3,
          h4 {
            color: $white;
          }
        }

        .map-info {
          min-height: 250px;
          width: 100%;
        }

        @include breakpoint(map-get($breakpoints, "mobile")) {
          .contact,
          .map-info {
            margin-bottom: 0;
            @include span(6 of map-get($susy, columns));
          }

          .map-info {
            @include last;
          }
        }
      }
```

### Drupal 8 doc by Sander
  * [documentation] (https://github.com/sqndr/d8-theming-guide)

### Performance
  * [Advagg](https://www.drupal.org/project/advagg) module
  * [page speed insights](https://github.com/Crosscheck/drupal-theme-boilerplate/issues/43) in grunt task
  * [minify](https://www.drupal.org/project/minify) of speedy module
