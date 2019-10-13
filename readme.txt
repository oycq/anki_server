# https://zhuanlan.zhihu.com/p/25042942

1.install dependances
sudo pip install webob PasteDeploy PasteScript sqlalchemy simplejson -i https://pypi.tuna.tsinghua.edu.cn/simple

2.install anki use zip
sudo pip install --upgrade setuptools
sudo easy_install AnkiServer-2.0.6.tar.gz

3.add user
ankiserverctl.py add

3.test
ankiserverctl.py debug

4.run
sudo ankiserverctl.py start

5.stop
sudo ankiserverctl.py stop

6.setting app
mysyncserver.py
import anki.sync
anki.sync.SYNC_BASE = 'http://47.100.76.211:27701/'
anki.sync.SYNC_MEDIA_BASE = 'http://47.100.76.211:27701/msync/'
