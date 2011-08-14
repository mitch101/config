%w{rubygems}.each do |lib| 
  begin 
    require lib 
  rescue LoadError => err
    $stderr.puts "Couldn't load #{lib}: #{err}"
  end
end

# Load project-specific .irbrc if it exists.
if Dir.pwd != File.expand_path("~")
  local_irbrc = File.expand_path '.irbrc'
  if File.exist? local_irbrc
    puts "Loading #{local_irbrc}"
    load local_irbrc
  end
end

# Prompt behavior
IRB.conf[:AUTO_INDENT] = true

# Loaded when we fire up the Rails console
# => Set a special rails prompt.   
if defined?(Rails.env)
  rails_env = Rails.env
  rails_root = File.basename(Dir.pwd)
  prompt = "#{rails_root}[#{rails_env.sub('production', 'prod').sub('development', 'dev')}]"
  IRB.conf[:PROMPT] ||= {}
  IRB.conf[:PROMPT][:RAILS] = {
    :PROMPT_I => "#{prompt}>> ",
    :PROMPT_S => "#{prompt}* ",
    :PROMPT_C => "#{prompt}? ",
    :RETURN   => "=> %s\n" 
  }
  IRB.conf[:PROMPT_MODE] = :RAILS
end