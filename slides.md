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

.notes quote by Gerry Lopez. He was talking about his experience big wave surfing. Fortunately for me, I can get this feeling from less life-threatening situations.

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
# Surfing

.notes What do you think of when I say surfing?

!SLIDE[bg=surfing/huntingtonbeach.png]
&nbps;

!SLIDE[bg=surfing/huntingtonbeach2.png]
&nbps;

!SLIDE[bg=surfing/slaterusopen.jpg]
&nbps;

!SLIDE[bg=surfing/slaterob.jpg]
&nbps;

!SLIDE[bg=surfing/alanascloset.jpg]
&nbps;

!SLIDE[bg=surfing/alanablanchard.jpg]
&nbps;

!SLIDE[bg=surfing/teahupoo.jpg]
&nbps;

.notes http://en.wikipedia.org/wiki/Teahupo'o

!SLIDE[bg=surfing/mavs.jpg]
&nbps;

!SLIDE[bg=surfing/jeffclark.jpg]
&nbps;

!SLIDE[bg=surfing/danereynolds.jpg]
&nbps;

!SLIDE[bg=surfing/rellsunn.jpg]
&nbps;

!SLIDE[bg=surfing/kassiameador.jpg]
&nbps;

.notes Growing up at Malibu and surfing there, I was able to see some of the best surfers in the world. I am a very visual person. That’s why I am into photography and I really enjoy films. So aesthetically, I will just like the way someone surfs, especially if they are smooth. That’s why I like how Joel (Tudor) surfs or someone like Dane Peterson. A smooth style is something that I appreciate and I want to emulate with my surfing. I really have a difficult time watching people surf when they are just “all over the place,” I just can’t visually accept it. (laughs)

!SLIDE[bg=surfing/hippies.jpg]
&nbps;

!SLIDE[bg=surfing/hippies2.jpg]
&nbps;

!SLIDE[bg=surfing/zenhippy.jpg]
&nbps;

!SLIDE[bg=surfing/treepose.png]
&nbps;

!SLIDE[bg=surfing/hampton-nh.jpg]
&nbps;

!SLIDE
# Kook
<table>
  <tr>
    <td>
      <img src="surfing/gettingup.jpg"/>
    </td>
    <td rowspan="100%">
      <img src="surfing/jacobkook.png"/>
    </td>
  </tr>
  <tr>
    <td>
      <img src="surfing/firstwaves.jpg"/>
    </td>
  </tr>
</table>

.notes Everyone starts as a beginner. But even the most experience surfers have kook moments

!SLIDE[bg=surfing/jettykooks.jpg]
# Kooking it up

.notes http://surfergrrrl.blogspot.com/2012/07/social-sunday-sloppy-surf-hmb-jetty.html

!SLIDE[bg=gerry/yoga.jpg]
# Gerry Lopez
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>
(not a Kook)

.notes You seem him talking in surf movies, and he's just so relaxed and Zen. I envy his vibe.

!SLIDE
# Surf is where you find it
![](gerry/book.jpg)

.notes So he wrote this book, and I got about halfway through it. And I picked it up again a week ago and suddenly I got to all the good stories. The ones that really talk about this hippy "Being Present" stuff

!SLIDE[bg=gerry/g-land.jpg] bullets incremental
# G-Land
* Grajagan Bay, Indonesia
* The ocean always wins

.notes Surf is where you find it page 128.  Gerry tells the story of riding giant unpredictable waves in G-Land. http://en.wikipedia.org/wiki/G-Land

!SLIDE
# We have kook moments in programming too

    @@@ruby bigcode
      if value == true
        return true
      else
        return false
      end

.notes Usually mine involve instance_eval and going down other overly complex rabbit holes when a simple Method or Class would do just fine. This is why we pair. But also, this is healthy. This is good for us.  The ocean always wins and humility is healthy.

!SLIDE[bg=ed/stylecrouch.jpg]
# Getting to the next level

!SLIDE[bg=scene/winter.jpg]
# Dedication

.notes I've taken many people out for their first surf. Or first few surfs. Only a few have truly taken to it.  Made it a priority.

!SLIDE[bg=scene/jenness.jpg]
# Priorities

!SLIDE bullets incremental
# The 5 Priorities
* Faith
* Health
* Family
* Friends
* Work

.notes I don't have the great big grey Gandalf beard up here to really sell this to you like it's a lifetime of wisdom. But I buy into it.

!SLIDE
# Faith = Surf
(of course)
[picture of me surfing]

.notes Faith means many thinks to different people. To me it's surfing.  It's that rare sense of connection with the universe.

!SLIDE
# Balance
[picture of beach yoga from after our wedding]

.notes this is an ordered list, but there are no absolutes.  Friends don't ALWAYS take priority over work. There is balance

!SLIDE
# The Buddha
[picture of the Buddha]

.notes The original Zen master.  Life story is basically. Extreme Decadence, Extreme Piety. The Middle Path.

!SLIDE
# Health
(Surfing is good for you)

[picture of J-Bird showing muscles?]

.notes good for your wrists

!SLIDE
# Family
(surf with your Family)

[picture of my Apple family]

!SLIDE
# Shiva

[picture of shiva stoked and padding]

.notes Not the indian God, just the middle name my Yoga-obsessed aunt gave to my cousin. Which he now goes by Took my on my first Surf. He was living in a shack his artist friend built, with ilegal plumbing. Over worked as an architect, on the fritz with his girlfriend at the time. Surfing every morning. Loving Life.

!SLIDE
# J-Bird

[picture of J-Bird on a sweet wave]

.notes My lifelong surf companion. My Wife. An Obsession with perfection.  And with surfing.
A roller-coaster of emotion as an Addict who rages at the need to surf. And is SOO excited when she finally catches that first wave. Her stoke never fades.

!SLIDE
# Friends
(surf with your Friends)

[picture of luke and other on beach]

!SLIDE
#Cynthia's Story
Surfing is My Drug

[picture of cynthia]

!SLIDE
#Chris's Story (the red)
keeps me sane (or less insane)

[picture of chris]

!SLIDE
#Post-Mango Surf

[picture of mangos]

!SLIDE
# Work
(surf before you go to work)

!SLIDE
# Ed

.notes I knew him as "Director of engineering". Opened my eyes to surfing new places, exploring. Surfing in the winter. Trying new boards One of the first time's Ed and I surfed together I can only recently started at Brontes.  He asked me "How are things"? I said "which, work? or surf?" He replied, oh well surf I guess. Clearly you understand what's more important.

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
(picture of grant twiggy baker)

!SLIDE
#Gerry's story of pipeline focus

!SLIDE
#Perrin's Story
patience
"No other thoughts in my head"

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

!SLIDE
#Presence

!SLIDE
Other sources of Presence
  - rock climbing
  - sky diving
  - vinyasa flow
  - meditation
  - music
  - "this guy holding his hands up to worship jesus"

!SLIDE
#Focus

!SLIDE
#Awareness

.notes listen to your body, pay attention to all your sense

!SLIDE
#Determination

!SLIDE
#Aspiration

.notes always try to be a better surfer, a better programmer, a better public speaker

!SLIDE
#Patience

!SLIDE
(quote from Gerry)

