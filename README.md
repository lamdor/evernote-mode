evernote-mode
=============
[![Gitter](https://badges.gitter.im/Join Chat.svg)](https://gitter.im/pymander/evernote-mode?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

Emacs interface for Evernote which originally started on
[Google Code][1].  Then it was [updated][2] for working with Ruby
1.9.3 and Emacs 24.1.  Which was then updated to [work with OAuth][3].
Then just a little bit of Emacs customization niceness was added.

INSTALLATION
------------

You will need to install the Evernote OAUTH Ruby gems in order to get
all of this stuff working.  Run the following command:

    gem install evernote_oauth

Clone this repo and run setup.rb:

    git clone https://github.com/pymander/evernote-mode
    cd evernote-mode/ruby
    ruby setup.rb

Copy `evernote-mode.el` to your load path.

See the [Original Readme][5] for installation and usage details.

CONFIGURATION
-------------

You'll need to get a production developer token from [Evernote][4] and
in Emacs set the custom variable `evernote-developer-token`.  If
`evernote-mode` is loaded this can be done easily with `M-x
customize-group evernote`.

TROUBLESHOOTING
---------------

If you get an error message regarding enclient.rb, you may need to modify
the variable enh-enclient-command in evernote-mode.el (check to see where setup.rb installed it).

[1]: http://code.google.com/p/emacs-evernote-mode/ "Original source"

[2]: https://github.com/rubbish/evernote-mode "rubbish/evernote-mode"

[3]: https://github.com/pymander/evernote-mode "pymander/evernote-mode"

[4]: http://dev.evernote.com/doc/articles/authentication.php#devtoken "Evernote Authentication"

[5]: doc/readme_en.html "Original Readme"
