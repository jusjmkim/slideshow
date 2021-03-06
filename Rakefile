require 'hoe'
require './lib/slideshow/cli/version.rb'

Hoe.spec 'slideshow' do

  self.version = SlideshowCli::VERSION

  self.summary = 'Slide Show (S9) - A Free Web Alternative to PowerPoint and Keynote in Ruby'
  self.description = summary

  self.urls     = ['https://github.com/slideshow-s9/slideshow']

  self.author  = 'Gerald Bauer'
  self.email   = 'webslideshow@googlegroups.com'

  self.extra_deps = [
    ['slideshow-models',   '>= 2.4.0'],   ## Note: pull in all deps via slideshow-models (e.g. props, textutils, etc.)
    ['slideshow-templates','>= 2.4.0'],
    ['gli', '>= 2.5.6']
    ## ['wikicloth', '>= 0.8.0']  make it a soft dependency   # mediawiki markup engine
    ## ['RedCloth','>= 4.2.9']    make it a soft dependency   # textile markup engine
  ]

  # switch extension to .markdown for gihub formatting
  self.readme_file  = 'README.md'
  self.history_file = 'HISTORY.md'

  self.licenses = ['Public Domain']

  self.spec_extras = {
    required_ruby_version: '>= 1.9.2'
  }


  self.post_install_message =<<EOS
******************************************************************************

Tip: Try some new template packs. Example:

  $ slideshow install impress.js
  
or
  
  $ slideshow install deck.js
  
and use like
  
  $ slideshow build welcome.text -t impress.js
  
or
  
  $ slideshow build welcome.text -t deck.js
 
or add some extra (plugins) helpers (left, right, etc). Example:
  
  $ slideshow install plugins

Questions? Comments? Send them along to the mailing list.
https://groups.google.com/group/webslideshow

******************************************************************************
EOS

end
