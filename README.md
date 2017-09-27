# wfmu-universe

### A [graph](https://markedg.github.io/wfmu-universe/) to show the musical relationships of WFMU DJs and playlists

This graph was produced by scraping the [WFMU DJ playlists](http://wfmu.org/playlists/) and using the doc2vec deep learning algorithm to train a neural network with a layer of 50 hidden nodes.  The subsequent learned weightings were reduced to two dimensions in order to make a visual representation of the musical neighborhood of WFMU.  Points that are close to each other are considered to have more similarities than those that are distant.  

Doc2Vec works best with a large volume of data, and the playlist data is perhaps not as substantial as would be optimal.  However, there are indications that neural net is finding genuine correspondences: there are a number of instances where a DJ is participating in more than one show, and these shows are often found very close to one another.  For instance, Hova's show is found close to "Greasy Kid Stuff", of which he is also one of the hosts. There is also a neighborhood of what might be termed Americana, with "The Antique Phonograph Music Program", "Thomas Edison's Attic", "Old Codger", and "The Radio Thrift Shop" all clustered together.

#### Next steps: 

It would be possible to validate the learnings of the neural net by withholding a segment of the playlists and comparing the similarity of groups of playlists by the same DJ.  Using this validation process would allow better tuning of the neural net parameters.
