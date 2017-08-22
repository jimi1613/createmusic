# Rudimentary AI Music Composer
The aim was to do a very basic AI music composer in 100 lines of code. This script takes a midi file and extracts just the notes, converting the piece into a large array of notes.

It uses the mido library for the handling of midi files and messages. The music I used was a Allegro con spirito by Mozart from [Classical Piano Midi Page](http://www.piano-midi.de/mozart.htm)

The model is built on Keras, using the LSTM layer. Since each note is a vector of pitch, velocity, and time, I trained the model to predict the next note given an array of n_prev previous notes (where n_prev is a parameter to be tuned).

Currently, it does not produce any intelligible music, but hopefully with some parameter tuning it could work a little better. It would probably help a lot to give it some help with musical theoretic features and syntax instead of letting it learn from just raw notes and timings. To do...

# 初级AI音乐作曲家
目的是在100行代码中做一个非常基本的AI音乐作曲家。 这个脚本需要一个midi文件，并且只提取笔记，将该片段转换成大量笔记。

它使用mido库来处理MIDI文件和消息。 我使用的音乐是莫扎特从[古典钢琴中篇]（http://www.piano-midi.de/mozart.htm）的Allegro con spirito

该模型建立在Keras上，使用LSTM层。 由于每个音符是音高，速度和时间的向量，所以我训练了模型以预测下一个音符，给出一个n_prev先前音符（其中n_prev是要调谐的参数）的数组。

目前，它不产生任何可理解的音乐，但希望通过一些参数调整可以更好地工作。 它可能会帮助很多东西给音乐理论的特点和语法一些帮助，而不是让它只从原始的笔记和时间学习。 去做...
