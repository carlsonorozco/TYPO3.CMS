=====================================================================
Feature: #34944 - PaginateViewHelper handles non-query-result objects
=====================================================================

Description
===========

The PaginateViewHelper accepts input collections of following types:
- :php:`QueryResultInterface`
- :php:`ObjectStorage`
- :php:`\ArrayAccess`
- :php:`array`

.. code-block:: html

	<f:widget.paginate objects="{blogs}" as="paginatedBlogs">
		<f:for each="{paginatedBlogs}" as="blog">
			<h4>{blog.title}</h4>
		</f:for>
	</f:widget.paginate>

..
