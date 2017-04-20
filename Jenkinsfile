stage ('test') {
  //gitHubPullRequestAddComment("hello")
  pullRequest['title'] = "This title was updated by Jenkins"
  pullRequest.comment("testing 123, 456")
  
  pullRequest['comments'].each { comment ->
    echo comment['body']
  }
}
