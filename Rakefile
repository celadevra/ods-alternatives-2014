task :default => [:compile]

task :compile do
  sh "pandoc -t slidy -s -i main.md -o ODS-alternatives.html"
  puts "HTML slide generated"
end

task preview: [:compile] do
  sh "open ODS-alternatives.html"
end
