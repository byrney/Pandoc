
directory 'out'

output='out/pandoc.md.html'
input='pandoc.md'
css='custom.css'


file output => [input, css] do
     cmd = "pandoc -c #{css} -o #{output} --self-contained #{input} "
     system(*cmd.split(' ')) || raise("ERROR: failed pandoc ")
end

task :default => ['out', output]

