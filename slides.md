!SLIDE center
# Hello!
![](jacob/pier.jpg)

!SLIDE[bg=jacob/lalancha.jpg]
# Jacob Burkhart

!SLIDE
# Engine Yard
![](jacob/coding.gif)

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

.notes 
Did you catch that?
How do you understand what's going on there?
Are you stepping through it line by line.  Metal Ruby Evaluator maybe?

!SLIDE
# Let's visualize

!SLIDE[bg=scene/headon.jpg]
&nbps;

!SLIDE bullets incremental
# Were you present?

.notes
call for audience participation

!SLIDE
# So what is surfing?

!SLIDE
# bikini babes and golden beaches?

!SLIDE
# monster waves

!SLIDE
# radical aerials

!SLIDE
# beach boys, jack johnson, dick dale

!SLIDE
# The beach bum

!SLIDE
# The "soul surfer"

!SLIDE
# Well I started here

!SLIDE
# The Kook

.notes
Everyone starts as a beginner. And even the most experience surfers have kook moments

!SLIDE
# Gerry Lopez

.notes
You seem him talking in surf movies, and he's just so relaxed and Zen.
I envy his vibe.

!SLIDE
# Surf is where you find it

.notes
So he wrote this book, and I got about halfway through it.
And I picked it up again a week ago and suddenly I got to all the good stories. The ones that really talk about this hippy "Being Present" stuff

!SLIDE
# Kook moment in big waves story
quote?

!SLIDE
# The ocean always wins

!SLIDE
# We have kook moments in programming too

TODO: think of anecdote kook moment in programming?

.notes
this is why we pair
but also, this is healthy. This is good for us.

!SLIDE
# Getting to the next level

!SLIDE
# Dedication

.notes
I've taken many people out for their first surf. Or first few surfs.
Only a few have truly taken to it.  Made it a priority.

!SLIDE
# Priorities

!SLIDE bullets incremental
# The 5 Priorities
* Faith
* Health
* Family
* Friends
* Work

# Balance

.notes
this is an ordered list, but there are no absolutes.  Friends don't ALWAYS take priority over work. There is balance

# The Buddha

.notes
The original Zen master.  Life story is basically. Extreme Decadence, Extreme Piety. The Middle Path.

# Number One Priority. Faith

.notes
It means many thinks to different people.
To me it's surfing.  It's that rare sense of connection with the universe.

# A Practice of Faith

# Shiva

.notes
Not the indian God, just the middle name my Yoga-obsessed aunt gave to my cousin. Which he now goes by
Took my on my first Surf.

He was living in a shack his artist friend built, with ilegal plumbing. Over worked as an architect, on the fritz with his girlfriend at the time. Surfing every morning. Loving Life.

# Ed

.notes
I knew him as "Director of engineering". Opened my eyes to surfing new places, exploring. Surfing in the winter. Trying new boards

One of the first time's Ed and I surfed together I can only recently started at Brontes.  He asked me "How are things"? I said "which, work? or surf?" He replied, oh well surf I guess. Clearly you understand what's more important.

# J-Bird

.notes
My lifelong surf companion. My Wife.
An Obsession with perfection.  And with surfing.
A roller-coaster of emotion as an Addict who rages at the need to surf. And is SOO excited when she finally catches that first wave.
Her stoke never fades.

# My surf lifestyle


# Wake up at 6


# In the water by 7


# Out by 9


# 10 am standup


# The Massive Lunch


# The Joy of Living

.notes
pair says: OMG this bug or this problem :-(
I say: OMG this bug! :-) It's so interesting. So intriguing. why why why. how how how.

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

# The long peeling waves

!SLIDE
# Sweet Sweet longboarding rides

!SLIDE
# Otters!

!SLIDE
# But the people :-(

!SLIDE
# Don't be Aggro!

.notes
PSA. Don't be the 1% that ruins surfing for the rest of us.
They are like the trolls on the internet, except instead of hiding behind anonymity they hide behind a facade of "being local", and "a better surfer than you".
But don't be an idiot either

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
#The Aloha spirit

.notes
Cheer for strangers. Share the waves.

!SLIDE
#???

#The hold down

#Big Waves

#Gerry's story of pipeline focus

#Perrin's Story
patience
"No other thoughts in my head"

#Chris's Story (the red)
keeps me sane (or less insane)

#Cynthia's Story
Jone-sing
My Drug

#Darren's Story
Interviewed at facebook. But you know, I have a pretty sweet life...

#Luke's Story
I'm not fat anymore!

!SLIDE bullets incremental
# Being Present
* focus
* awareness
* determination

# Gerry Lopez


!SLIDE[bg=beginners/stoked.jpg]
# Learn to Surf
