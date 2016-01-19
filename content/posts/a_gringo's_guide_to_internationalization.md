---
Category: 'DjangoCon 2012'
Copyright: 'Creative Commons Attribution license (reuse allowed'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=j2ZHZWfx60Y"'
Speakers: [Jacob Burch]
Tags: [django, internationalization]
ThumbnailUrl: 'http://i.ytimg.com/vi/j2ZHZWfx60Y/hqdefault.jpg'
Title: '"A Gringo''s Guide to Internationalization"'
date: '2012-09-04'
---
There's often a bubble in the English-speaking programming world that the
entire internet runs on English. Our Top-level domains are shortened english
words. Our programming languages--Python in particular--try to emulate English
words and grammar.

Firmly in place in this world for many years, my first attempt to translate a
pre-existing site came with a high sticker shock of nuanced difficulty. This
talk covers all the lessons I learned in taking a fully-fleshed web app with
no translation (and a programmer with no translation experience) to being
completely translated.

# Talk Overview

  1. Introduction to Translation
    1. Overview of gettext
    2. Brief history of a translation
      1. Add gettext calls
      2. `django-admin.py makemessages`
      3. Ship po file to translation service
      4. Receive file back
      5. Compile
      6. Fin
    3. gettext vs gettext_lazy
  2. Batteries Included
    1. gettext Python calls
    2. Middleware
    3. template tags
      1. trans vs. blocktrans
    4. Anti-patterns of the battery included use.
      1. Heavy whitespace in blocktrans
      2. Monster-sized translations
  3. The best laid plans of mice and men...
    1. Problems that get in the way of A history of a translation.
      1. Realize half the site is still untranslated
      2. Edit out the translations you already had translated to avoid re-curring costs
      3. Have the product adjust so two words change
      4. Realize common text that's in the database
      5. Fin?
    2. Patterns and tools to help
      1. `poxx.py` and the idea of a 'canonical' po file.
      2. `dbgettext`
      3. Wholly-translated template files (translate_include, trans_render)
  4. Advanced Translation Technique
    1. While undocumented, translation backend is pretty darn flexible and the source code is a treasure trove to make 'impossible' use cases not too bad.
    2. Overview of how the translation service works behind the scenes
      1. `_translation` thread local
      2. Merged translations (root->app->default)
      3. Sessions vs. Accept-Language
      4. Middleware and Context processors
    3. Example of advanced translation code: Multi-tenancy translation.
      1. Translating some sites, not translating others
      2. Translating Site A one way, Site B another
      3. Using an English translation for duct-tape and profit.
  5. Why Django's i18n sucks.
    1. In the vein of the "Django Sucks" Key note. It doesn't really, but it could use some changes--from minor to major.
    2. Why .po Files are archaic and limited.
    3. What we can do to improve for 1.5 and beyond.

