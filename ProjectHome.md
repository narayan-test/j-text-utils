Gives text representations of common data views such as tree and table.
<br>
<br>
<b>A table example:</b>
<pre><code>______________________________________________________________
| First Name| Last Name| Sport        | # of Years| Vegetarian|
|=============================================================|
| Jane      | White    | Speed reading| 20        | true      |
| Joe       | Brown    | Pool         | 10        | false     |
| John      | Doe      | Rowing       | 3         | true      |
| Kathy     | Smith    | Snowboarding | 5         | false     |
| Sue       | Black    | Knitting     | 2         | false     |
</code></pre>
<br>
<br>
Read<br>
<a href='http://code.google.com/p/j-text-utils/wiki/UsingTextTable'>Using TextTable</a>
to see how it is done.<br>
<br>
<br>
<br>
<b>A tree example:</b>
<pre><code>-- target/
   |-- j-text-utils-0.3.jar
   |-- maven-archiver/
   |   `-- pom.properties
   |-- classes/
   |   `-- dnl/
   |      `-- utils/
   |         `-- text/
   |            |-- TextTreeTable$TreeTableSeparatorPolicy.class
   |            |-- SeparatorPolicy.class
   |            |-- TextTable.class
   |            |-- TextTreeTable.class
   |            |-- TextTableRenderer.class
   |            |-- tree/
   |            |   `-- TextTree.class
   |            |-- TextTableModel.class
   |            |-- TextTreeTable$1.class
   |            |-- LastRowSeparatorPolicy.class
   |            `-- TextTreeTableRenderer.class
   |-- test-classes/
   |   `-- dnl/
   |      `-- utils/
   |         `-- text/
   |            |-- TextTreeTableTest.class
   |            |-- TextTableTest.class
   |            `-- tree/
   |               |-- FsObject.class
   |               |-- TextTreeTest.class
   |               `-- FsModel.class
   `-- surefire-reports/
      |-- dnl.utils.text.TextTreeTableTest.txt
      |-- TEST-dnl.utils.text.tree.TextTreeTest.xml
      |-- TEST-dnl.utils.text.TextTreeTableTest.xml
      |-- TEST-dnl.utils.text.TextTableTest.xml
      |-- dnl.utils.text.TextTableTest.txt
      `-- dnl.utils.text.tree.TextTreeTest.txt
</code></pre>

Example Code:<br>
<a href='http://code.google.com/p/j-text-utils/wiki/UsingTextTree'>Using TextTree</a>

<hr />


<h3>Adding j-text-utils to your Maven POM</h3>

The dependency:<br>
<pre><code>&lt;dependency&gt;
	&lt;groupId&gt;dnl.utils&lt;/groupId&gt;
	&lt;artifactId&gt;j-text-utils&lt;/artifactId&gt;
	&lt;version&gt;0.3.3&lt;/version&gt;
&lt;/dependency&gt;
</code></pre>

And add the following repository:<br>
<pre><code>&lt;repositories&gt;
	&lt;repository&gt;
		&lt;id&gt;d-maven&lt;/id&gt;
		&lt;url&gt;http://d-maven.googlecode.com/svn/trunk/repo&lt;/url&gt;
	&lt;/repository&gt;
&lt;/repositories&gt;
</code></pre>
<hr />
<b>'Provided' dependencies:</b>
<br><br>
Note that if you use the <code>GuavaTableModel</code> you'll need to add a dependency for guava in your pom.<br>
<br>Same goes for CSV functionality which requires opencsv, for example:<br>
<pre><code>&lt;dependency&gt;
	&lt;groupId&gt;net.sf.opencsv&lt;/groupId&gt;
	&lt;artifactId&gt;opencsv&lt;/artifactId&gt;
	&lt;version&gt;2.3&lt;/version&gt;
&lt;/dependency&gt;
</code></pre>