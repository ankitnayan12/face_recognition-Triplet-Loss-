# face_recognition-Triplet-Loss-
Model training aims to learn an embedding  f(x)  of image  x  such that the squared L2 distance between all faces of the same identity is small and the distance between a pair of faces from different identities is large. This can be achieved with a triplet loss  L  that is minimized when the distance between an anchor image  xai  and a positive image  xpi  (same identity) in embedding space is smaller than the distance between that anchor image and a negative image  xni  (different identity) by at least a margin  α .

L=∑i=1m[∣∣f(xai)−f(xpi))∣∣22−∣∣f(xai)−f(xni))∣∣22+α]+
