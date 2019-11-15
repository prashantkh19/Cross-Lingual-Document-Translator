# Cross-Language-Document-Translator

### IBM Model 1 Algorithm

![image](https://user-images.githubusercontent.com/27685757/68961093-85b88380-07f7-11ea-83a8-ed1c764b1a41.png)

### Flow of Algorithm
`train` method is called initially which internally calls `train_iter_helper`. In `train_iter_helper` the count dictionary is made which is used to update the translation model. The translation model gets updated using E-M Method. Model generates Translation table which ultimately is improvised with given number of iterations.

Then translation method `translate_sentence` is called for given trained model which ultimately gives us translated document. It tokenizes the source sentence and gets the corresponding translated word (assuming they map continuously with no distortion) and returns final sentence.
