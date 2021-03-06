'cram-mode.el' provides a major mode for the `cram <https://pypi.python.org/pypi/cram>`_ files.
Mode adds syntax highlighting and interactive commands to run cram against
buffer or region.
``cram-mode`` is automatically enabled for files with '.t' extension.

.. image:: asciicast.gif

Installation
------------

Package is not present in any of known package archives.

Installation procedure for `Spacemacs <http://spacemacs.org>`_

- Add package to the ``dotspacemacs-additional-packages``::

   dotspacemacs-additional-packages `(
    (cram-mode :location (recipe :fetcher github :repo "signalpillar/cram-mode"))
   )

- Add ``(require 'cram-mode)`` in ``dotspacemacs/user-config`` body.

Key bindings
------------

::

  | Key binding | Command                  | Description                                                     |
  |-------------+--------------------------+-----------------------------------------------------------------|
  | C-c C-b     | cram-run-buffer-in-debug | Run 'cram -d' against current buffer.                           |
  | C-c C-r     | cram-run-region-in-debug | Run 'cram -d' against region and insert output below selection. |
