Table of Contents Tree Test
===========================

Sphinx에서는 table of contents를 이용해서 문서 사이의 관계를 정의할 수 있다.

.. seealso::

   공식 홈페이지: `toctree <https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html>`_


toctree
-------

**예시** ::

   .. toctree::

      toctree1
      _tree/toctree2
      toctree3

.. toctree::

   toctree1
   _tree/toctree2
   toctree3


caption
-------

| caption으로 toctree에 대한 설명을 추가할 수 있다.
| 또한 name을 설정하면 다른 곳에서 name으로 referencting이 가능하다.
| code: ``toctree referencing :ref:`basic-example`.``
| toctree referencing :ref:`basic-example`.

**예시** ::

   .. toctree::
      :caption: Content trees
      :name: basic-example

      toctree1
      _tree/toctree2
      toctree3

.. toctree::
   :caption: Content trees
   :name: basic-example

   toctree1
   _tree/toctree2
   toctree3


maxdepth
--------

maxdepth로 table의 depth를 조절할 수 있다.

**예시** ::

   .. toctree::
      :maxdepth: 2

      toctree1
      _tree/toctree2
      toctree3

.. toctree::
   :maxdepth: 2

   toctree1
   _tree/toctree2
   toctree3


numbered
--------

contenct에  번호를 매길 수도 있다. 전체 문서에 numbered가 적용되어 결과값은 출력하지 않는다. 

**예시** ::

   .. toctree::
      :numbered:

      toctree1
      _tree/toctree2
      toctree3


globbing
--------

globbing을 사용하여, 매칭된 document들을 전부 추가할 수도 있다.

**예시** ::

   .. toctree::
      :glob:

      toctree*

.. toctree::
   :glob:

   toctree*

