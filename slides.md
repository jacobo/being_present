!SLIDE[bg=scene/headon.jpg]
&nbps;

!SLIDE center
# Hello!
![](jacob/pier.jpg)

!SLIDE[bg=jacob/lalancha.jpg]
# Jacob Burkhart

!SLIDE
![](logos/engine-yard.png)
![](jacob/coding.gif)

!SLIDE center
# What is presence?

!SLIDE center
# Awareness

!SLIDE center
# Mindfulness

!SLIDE center
# Focus

!SLIDE center align-left
## Such is the life we can know.
## Living in the past and in the future - in recollection and in anticipation - creates a less clear picture of the present.
## By being in the here and now we understand that the past and future only exist in the present.
## That's all there is, but speaking for myself, I couldn't ask for more.

.notes quote by Gerry Lopez

!SLIDE
# Gerry Lopez

!SLIDE
    @@@ruby
    def traversal_from_hash(from_hash)
      traversal = Proc.new do |hash_a, hash_b, opts1|
        a_vals = []
        b_vals = []
        sub_procs = [Proc.new{ "" }]
        hash_a.each do |key, value|
          if (value.is_a?(Hash) && hash_b[key].is_a?(Hash))
            sub_procs << Proc.new do |opts2|
              traversal.call(value, hash_b[key], opts2)
            end
          else
            unless hash_b[key].nil?
              a_vals << value
              b_vals << hash_b[key]
            end
          end
        end
        sub_proc = Proc.new do |opts3|
          sub_procs.collect do |sp|
            sp.call(opts3)
          end.join("")
        end
        a_vals.uniq.collect do |a_val|
          yield a_val, b_vals, sub_proc, opts1
        end
      end
    end

.notes Did you catch that? How do you understand what's going on there? Are you stepping through it line by line.  Mental Ruby Evaluator maybe?

!SLIDE  center
# Surf Culture

.notes What do you think of when I say surfing?

!SLIDE[bg=surfing/waikiki.jpg]
&nbps;

!SLIDE[bg=surfing/mavs.jpg]
&nbps;

!SLIDE[bg=surfing/beachboys.jpg]
&nbps;

!SLIDE[bg=surfing/jordysmithaerial.jpg]
&nbps;

!SLIDE[bg=surfing/slaterob.jpg]
&nbps;

!SLIDE[bg=surfing/fasttimes.jpg]
&nbps;

!SLIDE[bg=surfing/treepose.png]
&nbps;

!SLIDE
# Well I started here

!SLIDE
# The Kook

.notes Everyone starts as a beginner. And even the most experience surfers have kook moments

!SLIDE
# Gerry Lopez

.notes You seem him talking in surf movies, and he's just so relaxed and Zen. I envy his vibe.

!SLIDE
# Surf is where you find it

.notes So he wrote this book, and I got about halfway through it. And I picked it up again a week ago and suddenly I got to all the good stories. The ones that really talk about this hippy "Being Present" stuff

!SLIDE
# Kook moment in big waves story
quote?

!SLIDE
# The ocean always wins

!SLIDE
# We have kook moments in programming too

.notes this is why we pair. but also, this is healthy. This is good for us. TODO: think of anecdote kook moment in programming?

!SLIDE
# Getting to the next level

!SLIDE
# Dedication

.notes I've taken many people out for their first surf. Or first few surfs. Only a few have truly taken to it.  Made it a priority.

!SLIDE
# Priorities

!SLIDE bullets incremental
# The 5 Priorities
* Faith
* Health
* Family
* Friends
* Work

!SLIDE
# Balance

.notes this is an ordered list, but there are no absolutes.  Friends don't ALWAYS take priority over work. There is balance

!SLIDE
# The Buddha

.notes The original Zen master.  Life story is basically. Extreme Decadence, Extreme Piety. The Middle Path.

!SLIDE
# Number One Priority. Faith

.notes It means many thinks to different people. To me it's surfing.  It's that rare sense of connection with the universe.

!SLIDE
# A Practice of Faith

!SLIDE
# Shiva

.notes Not the indian God, just the middle name my Yoga-obsessed aunt gave to my cousin. Which he now goes by Took my on my first Surf. He was living in a shack his artist friend built, with ilegal plumbing. Over worked as an architect, on the fritz with his girlfriend at the time. Surfing every morning. Loving Life.

!SLIDE
# Ed

.notes I knew him as "Director of engineering". Opened my eyes to surfing new places, exploring. Surfing in the winter. Trying new boards One of the first time's Ed and I surfed together I can only recently started at Brontes.  He asked me "How are things"? I said "which, work? or surf?" He replied, oh well surf I guess. Clearly you understand what's more important.

!SLIDE
# J-Bird

.notes My lifelong surf companion. My Wife. An Obsession with perfection.  And with surfing.
A roller-coaster of emotion as an Addict who rages at the need to surf. And is SOO excited when she finally catches that first wave. Her stoke never fades.

!SLIDE
# My surf lifestyle

!SLIDE
# Wake up at 6

!SLIDE
# In the water by 7

!SLIDE
# Out by 9

!SLIDE
# 10 am standup

!SLIDE
# The Massive Lunch

!SLIDE
# The Joy of Living

.notes pair says: OMG this bug or this problem :-( I say: OMG this bug! :-) It's so interesting. So intriguing. why why why. how how how.

!SLIDE
# Surf Safari on the Weekends

!SLIDE
# Beach Boys: 
Lets go surfin now
Everybodys learning how
Come on and safari with me

!SLIDE
# We have a great coastline
Marin county
The usual weekday breaks
State Parks
Santa Cruz

!SLIDE
# ahh Santa Cruz

!SLIDE
# The long peeling waves

!SLIDE
# Sweet Sweet longboard rides

!SLIDE
# Otters!

!SLIDE
# But the people :-(

!SLIDE
# Don't be Aggro!

.notes PSA. Don't be the 1% that ruins surfing for the rest of us. They are like the trolls on the internet, except instead of hiding behind anonymity they hide behind a facade of "being local", and "a better surfer than you". But don't be an idiot either

!SLIDE
# Surf etiquette

!SLIDE
#Don't drop in!

!SLIDE
#Priority to the peak

!SLIDE
#Control your board

!SLIDE
#Accidents happen

!SLIDE
#Ding Repair
(picture of Rich)

!SLIDE
#The Aloha spirit

.notes Cheer for strangers. Share the waves.

!SLIDE[bg=beginners/stoked.jpg]
# Learn to Surf

Goofy or Regular

paddling

the pop up

cover your head

hold your breath

!SLIDE
#The hold down

!SLIDE
#Gerry's story of 3 wave hold down

!SLIDE
#Big Waves

!SLIDE
#Mavericks

!SLIDE
#Don't panic after you've panic'd

!SLIDE
#Gerry's story of pipeline focus

!SLIDE
#Perrin's Story
patience
"No other thoughts in my head"

!SLIDE
#Chris's Story (the red)
keeps me sane (or less insane)

!SLIDE
#Cynthia's Story
Surfing is My Drug

!SLIDE
#Darren's Story
Interviewed at facebook. But you know, I have a pretty sweet life...

!SLIDE
#Priorities!

!SLIDE
#Be ready when the surf is up

!SLIDE
#Be patient when it's not

!SLIDE
#Find your style

