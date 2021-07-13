# Image-recognition-of-fashion-items-in-CNN-configuration-using-keras__Tensorflow_and_Keras__

Kerasを用いて、ファッションアイテムの画像認識を行いました。

構成は簡単なもので、入力層から畳み込み層、Flatten層を通して全結合層（Dense）という構成になっています。  

今回はepoch数を30とし、早期終了を行うEarlyStoppingを生成しましたが、実行する際に、ストップすることはありませんでした。  

【考察】  
5エポック以降は損失、正解率共にほぼ横ばいになっています。  
しかし、訓練データの損失は5エポック以降も下がり続け、正解率は上昇を続けています。ドロップアウトを適用しましたが、若干のオーバーフィッティングが発生していると考えられます。  
この解決法として正則化が考えられます。  

***
.ipynbファイルが開かれない時は、こちらのリンクにURLを貼ってご覧になってください。  
[nbviewer](https://nbviewer.jupyter.org/)
