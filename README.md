# Strepkills
Visit http://strepsils.herokuapp.com/game to play
Join our chatroom [here](http://strepsils.herokuapp.com/)
Current version: 1.0.0

### What is Strepkills?
Strepkills was made as a one week group challenge- it aims to be a multiplayer game with a real-time chat and minimalist gameplay. It can be played on your browser and features your player avatar (or a 'strepsil') which is matched up with other player controlled avatars vying for dominion over the board.

### Our one-line goal
> A real-time browser-based game which facilitates multiple players on individual clients.

### Prerequisites
- Ruby v 2.4.1

  get the latest verson here: https://www.ruby-lang.org/en/downloads/
  
- PostgreSQL v10.1

  get here: https://gist.github.com/sgnl/609557ebacd3378f3b72

### Running on localhost

```sh
$ git clone https://github.com/Xin00163/mmog.git
$ cd mmog
$ bundle install
$ rails db:create
$ rails db:migrate
$ rails s
go to http://localhost:3000 in browser
```

To run tests:
```
$ rspec
```

### Technologies
| Tech | Description |
| ------ | ------ |
| [Ruby on Rails](http://rubyonrails.org/) | To create a website to host games |
| [ActionCable](http://guides.rubyonrails.org/action_cable_overview.html) | Integrates WebSockets with Rails |
| [Redis gem](https://redis.io/) | In-memory data-structure store and cache |
| [Rubyracer gem](https://github.com/cowboyd/therubyracer) | Evaluates and reads JS and Ruby |
| [PostgreSQL](https://www.postgresql.org/) | Database of choice |
| [RSpec](http://rspec.info/) | Testing framework for Ruby code |

### Creation to release

* Keeping scalability in mind we created a game hub website, to easily host many different games in the future and to provide players with their individual profiles.
* During the conception of the game our team decided to use the fewest number of pre-created frameworks as possible, and as a result we made an original game framework from scratch.
* Our starting point was creating a chatroom using ActionCable to simultaenously send mesages to multiple users, and we applied the same methodology to our game.
* As a result Strepkills incorporates WebSockets for seamless connections and after many iterations of improvements it is optimised for fast, responsive gameplay.  

### Our team
[Keran](https://github.com/ker-an), [Rhys](https://github.com/rskyte), [Tim](https://github.com/Le5tes), [Varun](https://github.com/VarunCodes), [Xin](https://github.com/Xin00163)
Honourary tester: Umair

View our end-of-week presentation here- http://slides.com/rspecgod/strepsil-wars#/
