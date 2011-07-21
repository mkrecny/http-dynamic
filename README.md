# http-dynamic -- execute any script over HTTP

## Note

This is an experiment. It is not performant! Do not use in production.

## Usage

Start http-dynamic
<pre>
  ./lib/http-dynamic
</pre>

Put scripts (ruby, python, php) in the ./scripts directory:

scripts/hello.rb
<pre>
	puts 'hello from ruby'
	puts 'arguments are '+ ARGV[0]
	exit()
</pre>

And execute over HTTP:
<pre>
	curl localhost:8080/hello.rb?foo=bar
</pre>
Should output:
<pre>
	hello from ruby
	arguments are foo=bar
</pre>		
(all data written to stdout will be buffered and returned to HTTP client when script exits)