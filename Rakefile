
directory 'out'

html='out/pandoc.md.html'
docx='out/pandoc.md.docx'
input='pandoc.md'
css='custom.css'

file html => [input, css] do
     cmd = "pandoc -c #{css} -o #{html} --self-contained #{input} "
     system(*cmd.split(' ')) || raise("ERROR: failed pandoc ")
end

file docx => [input] do
     cmd = "pandoc -o #{docx} --self-contained #{input} "
     system(*cmd.split(' ')) || raise("ERROR: failed pandoc docx")
end

task :default => ['out', html]
task :docx => ['out', docx]

task :bundle do
     system("bundle", "check") || system("bundle", "install")
end

desc 'first time only setup tasks'
task :setup => [:bundle]
