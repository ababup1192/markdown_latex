task :default => ["build",  'clean', 'open']

name = "paper"

task :build do
  Dir.glob("src/*.md").map { |md|
    tex = md.sub(".md",  ".tex")
    `pandoc #{md} -o #{tex}`
  }

  #puts `bibtex #{name}.aux`
  puts `platex -kanji=UTF8 src/#{name}.tex`
  puts `dvipdfmx #{name}.dvi`
  puts `mv #{name}.pdf build/`
end

task :clean do
  Dir.glob("src/*.md").map { |md|
    tex = md.sub(".md",  ".tex")
    if md != 'src/paper.tex'
      `rm #{tex}`
    end
  }

  `rm *.log`
  `rm *.aux`
  `rm *.dvi `
end

task :open do
  `open build/paper.pdf`
end
