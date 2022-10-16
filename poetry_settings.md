### poetryの.venvをvscodeに認識させて動かすまでの手順

- poetry initでプロジェクトスタート、適当にパッケージをaddする
- poetry config --listでconfigを確認して、
- virtualenvs.in-project = trueとなっていることを確かめる
- まず、poetry installすると今いるディレクトリ下に{cache-dir}/virtualenvsが生成される
- poetry env listでactivatedかどうかを確かめられる
- 重要!!!:projectのディレクトリにいることを確かめた上で、poetry shellすると.venvに入れる
- ただ、vscode上のterminalがiTermの方と別のウィンドウで開かれてるせいで今までうまく行ってなかったぽい
- vscodeの方のterminalで、きちんと直下の.venvにpoetry shellで入れば解決！interpreterを選ばずに済む
- python ~~.pyで動くか確認する







