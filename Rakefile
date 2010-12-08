require 'ant'

task :init do
  mkdir_p "build"
end

task :build => :init do
  ant.javac :srcdir => "src", :destdir => "build", :classpath => "lib/dx.jar"
end

task :clean do
  rm_rf "build"
end

task :default => :build