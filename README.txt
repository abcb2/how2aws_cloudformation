■テンプレート集
http://aws.amazon.com/jp/cloudformation/aws-cloudformation-templates/

■自学自習のヒント
http://d.hatena.ne.jp/torazuka/20140709/cfn

■opsworksとcloudformation
http://dev.classmethod.jp/cloud/create-opsworks-by-cloudformation/
http://aws.amazon.com/jp/opsworks/faqs/
http://aws.amazon.com/jp/cloudformation/faqs/


-------------------------
■検証方法
・cloudformerを立ち上げて自分の環境をjsonに変換。
・それを小さなパーツからコツコツと。
・aws cloudformation create-stack --generate-cli-skeleton > tmp/skeleton.json　している
　が、それを使ってaws cloudformation create-stack --cli-input-json file://hoge.jsonして
　成功するサンプルはまだない。

・下記はcloudformerから抜粋したjsonを使っての実行
$ aws cloudformation create-stack --stack-name hoge --template-body file://01.json 
