task :default => [:compile]

task :compile do
  sh "pandoc -t slidy -s -i --template=default.slidy --bibliography=master.bib --csl=gb7714.csl main.md -o ODS-alternatives.html"
  puts "HTML slide generated"
end

task preview: [:compile] do
  sh "open ODS-alternatives.html"
end
