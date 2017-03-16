node{
    def workspace = pwd()
    
    
    stage('Read template'){
	    def templText = readFile("${workspace}@script/email-template.html")
	    def engine = new groovy.text.SimpleTemplateEngine()
	    def templ = engine.createTemplate(templText)
	    
	    def foo = "My Foo"
	    def bar = "My Bar"
	    emailText = templ.make([foo:foo, bar:bar]).toString()
	    
	    echo(emailText)
	    echo("Something else ${foo} and ${bar}")
    }
	stage('Send email'){
	}
}
