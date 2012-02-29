!SLIDE subsection
# Sass

!SLIDE red
# Syntactically
# Awesome
# Style
# Sheets

!SLIDE
# Sass er en utvidelse av CSS3
<!-- NOTE Sei noke om css superset osv -->

!SLIDE bullets incremental
# Sass gir deg:
* Kraftigere syntax
* Bedre abstraksjoner
* Organisering!

<!-- NOTE organisering i "partials" og plugins/pakker -->

!SLIDE bullets incremental
# Utvidelser av CSS3:
* Nøsting
* Variabler
* Arv
* Mixins
* Partials

!SLIDE bullets incremental
# Utvidelser av CSS3:
* Funksjoner
* Kondisjoner/loops
* Kalkulasjoner
* Minifisering
* ..og mer!

!SLIDE
#Rett på kode :)

!SLIDE
# Nøsting

!SLIDE
#SASS
    @@@ css
    .annonse {
      float: left;

      span {
        color: red;
        
        &:hover{
        	color: blue;
        }
      }
    }

!SLIDE
#CSS
    @@@ css
    .annonse {
      float: left;
    }
    .annonse span {
        color: red;
    }
    .annonse span:hover{
    	color: blue;
    }

!SLIDE
# Variabler

!SLIDE
#SASS
    @@@ css
    $boxWidth: 40px;

    .small{
    	width: $boxWidth;
    }

    .big{
    	width: $boxWidth * 2;
    }

!SLIDE
#CSS
    @@@ css
    .small{
    	width: 40px;
    }

    .big{
    	width: 80px;
    }



!SLIDE
# Mixins

!SLIDE
#SASS
    @@@css
    @mixin horizontal-list($spacing: 10px) {
      li {
        float: left;
        margin-right: $spacing;
      }
    }

!SLIDE

    @@@css
    #footer ul.nav {
      @include horizontal-list(20px);
      margin-top: 1em;
    }

!SLIDE
#CSS
	@@@css
    #footer ul.nav {
    	margin-top: 1em;
    }

    #footer ul.nav li{
    	float: left;
    	margin-right: 20px;
    }


!SLIDE
# CSS 3

!SLIDE
#SASS
    @@@css
    .rounded {
      @include border-radius(4px, 4px);
    }

!SLIDE
#CSS
    @@@css
    .rounded {
      -webkit-border-radius: 4px 4px;
      -moz-border-radius: 4px / 4px;
      -o-border-radius: 4px / 4px;
      -ms-border-radius: 4px / 4px;
      -khtml-border-radius: 4px / 4px;
      border-radius: 4px / 4px;
    }