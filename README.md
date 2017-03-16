# jenkins-email-template-test
A PoC on how to use email templates for email notifications in Jenkins pipeline jobs.

# Jenkins script approvals needed

Requires the following approvals:

    groovy.text.Template make java.util.Map
    groovy.text.TemplateEngine createTemplate java.lang.String
    new groovy.text.SimpleTemplateEngine
