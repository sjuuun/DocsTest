Insertion Test of Sphinx
=========================

Insert on document


Short Paragraph
---------------

Literal block 처럼 작은 문단을 삽입할 수 있다.
note, warning, versionadded, versionchanged, deprecated, seealso 등 다양하게 존재한다.

.. seealso::

   Sphinx documentation: 
   `Paragraph-level markup <https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#paragraph-level-markup>`_

**예시** ::

   .. warning::
      example warning paragraph

.. warning::
   example warning paragraph


Footnotes
---------

각주 및 인용구를 넣을 수 있다.

**예시** ::

   각주는 ``[#각주이름]_`` 으로, 인용구는 ``[Ref]_`` 로 넣을 수 있습니다.
   예를 들어, 각주는 [#f1]_ 으로, 인용구는 [Ref]_ 로 넣습니다.

   .. [#f1] 예시 각주 1
   .. [Ref] 예시 인용구

| 각주는 ``[#각주이름]_`` 으로, 인용구는 ``[Ref]_`` 로 넣을 수 있습니다.
| 예를 들어, 각주는 [#f1]_ 으로, 인용구는 [Ref]_ 로 넣습니다.


Table
------

두 가지 방법으로 표를 삽입할 수 있다.

* Grid table ::

   +-----+---+---+----+
   | mul | 2 | 3 | 4  |
   +=====+===+===+====+
   | 2   | 4 | 6 | 8  |
   +-----+---+---+----+
   | 3   | 6 | 9 | 12 |
   +-----+---+---+----+

+-----+---+---+----+
| mul | 2 | 3 | 4  |
+=====+===+===+====+
|  2  | 4 | 6 | 8  |
+-----+---+---+----+
|  3  | 6 | 9 | 12 |
+-----+---+---+----+

* Simple table ::

   ===== ===== =======
   A     B     A and B
   ===== ===== =======
   False False False
   False True  False
   True  False False
   True  True  True
   ===== ===== =======

===== ===== =======
A     B     A and B
===== ===== =======
False False False
False True  False
True  False False
True  True  True
===== ===== =======


Image
-----

이미지를 삽입할 수 있다.

**예시** ::

   .. image:: _image/github.jpg

.. image:: _image/github.jpg


Hyperlink
---------

```링크 텍스트 <링크 주소>`_`` 로 하이퍼링크를 삽입할 수 있다.

**예시** ::

   `Read the Docs <https://readthedocs.org>`_

**결과**

`Read the Docs <https://readthedocs.org>`_


Download
--------

source tree 안에 있는 파일을 다운받게 할 수도 있다.
다운로드 가능한 파일들은 _downloads 라는 subdirectory 안에 있어야 한다.

예시 ::

   다운로드 :download: `예시 파일 <_downloads/msg.py>` .

다운로드 :download:`예시 파일 <_downloads/msg.py>`


---------------


.. [#f1] 예시 각주 1
.. [Ref] 예시 인용구

