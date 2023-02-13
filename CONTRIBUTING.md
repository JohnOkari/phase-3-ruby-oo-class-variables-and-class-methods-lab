# Contributing to Learn.co Curriculum

We're really exited that you're about to contribute to the [open curriculum](https://learn.co/content-license) on [Learn.co](https://learn.co). If this is your first time contributing, please continue reading to learn how to make the most meaningful and useful impact possible.

## Raising an Issue to Encourage a Contribution

If you notice a problem with the curriculum that you believe needs improvement
but you're unable to make the change yourself, you should raise a Github issue
containing a clear description of the problem. Include relevant snippets of
the content and/or screenshots if applicable. Curriculum owners regularly reviewclass Song
  attr_accessor :name, :artist, :genre

  @@count = 0
  @@artists = []
  @@genres = []

  def initialize(name, artist, genre)
    @name = name
    @artist = artist
    @genre = genre
    @@count +=1
    @@genres << genre
    @@artists << artist
  end

  def self.count
    @@count
  end

  def self.artists
    @@artists.uniq
  end

  def self.artist_count
    artist_count = {}
    @@artists.each do |artist|
      if artist_count[artist]
        artist_count[artist] += 1 
      else
        artist_count[artist] = 1
      end
    end
    artist_count
  end

  def self.genres
    @@genres.uniq
  end

  def self.genre_count
    genre_count = {}
    @@genres.each do |genre|
      if genre_count[genre]
        genre_count[genre] += 1 
      else
        genre_count[genre] = 1
      end
    end
    genre_count
  end
end
issue lists and your issue will be prioritized and addressed as appropriate.

## Submitting a Pull Request to Suggest an Improvement

If you see an opportunity for improvement and can make the change yourself go
ahead and use a typical git workflow to make it happen:

* Fork this curriculum repository
* Make the change on your fork, with descriptive commits in the standard format
* Open a Pull Request against this repo

A curriculum owner will review your change and approve or comment on it in due
course.

# Why Contribute?

Curriculum on Learn is publicly and freely available under Learn's
[Educational Content License](https://learn.co/content-license). By
embracing an open-source contribution model, our goal is for the curriculum
on Learn to become, in time, the best educational content the world has
ever seen.

We need help from the community of Learners to maintain and improve the
educational content. Everything from fixing typos, to correcting
out-dated information, to improving exposition, to adding better examples,
to fixing tests—all contributions to making the curriculum more effective are
welcome.
