
guard :rake, :task => :default do
    watch('pandoc.md')
    watch('custom.css')
    watch('Rakefile')
end

guard :livereload, grace_period: 0.5 do
  watch(%r{out/.+\.(css|js|html)$})
end
