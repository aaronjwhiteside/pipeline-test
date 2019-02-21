properties([
  pipelineTriggers([
    issueCommentTrigger('.*build me.*')
  ])
])

node {
stage ('pre-test') {
}
}

node {

stage ('test') {
  //gitHubPullRequestAddComment("hello")
//  pullRequest['title'] = "This title was updated by Jenkins, testing 123"
  pullRequest.setLabels(['bug', 'duplicate'])
  pullRequest.removeLabel('bug')

  echo "Labels: ${pullRequest.getLabels().collect()}"
  
  pullRequest.setBody(pullRequest.getBody() + '\nhello world \nweeeeeee abc')
  
//        authors = []
//        for (commit in pullRequest.commits) {
//           authors.push(commit.author)
//           authors.push(commit.committer)
//        }
//        authors = authors.unique().join(' ')
//  echo "Unique Authors: ${authors}"
  
//  pullRequest.comment("testing 123, 456")
//  pullRequest.reviewComment(pullRequest['head'], 'Jenkinsfile', 2, 'why is this commented out?')
//  pullRequest.createStatus(status: 'success', context: 'Pipeline', description: 'Wooohooo!')
def myUrl = "https://www.google.com"
pullRequest.createStatus(status: 'success',
            context: 'continuous-integration/jenkins/pr-merge/validation',
            description: 'Project passed all validations',
            targetUrl: "${myUrl}")
  
//    if (pullRequest.commits) {
//        for (commit in pullRequest.commits) {
//            if (commit.sha == env.GIT_COMMIT) {
//                for (commitFile in commit.files) {
//                    echo "SHA: ${commitFile.sha} File Name: ${commitFile.filename} Status: ${commitFile.status}"
//                    if (!(commitFile.filename ==~ /\w\s+kubernetes\\/.+/)) {
//                        echo "HOORAAY"
//                    }
//                }
//            }
//        }
//    }  
  
//  pullRequest['locked'] = !pullRequest['locked']
  
//  for (assignee in pullRequest['assignees']) {
//    echo assignee
//  }
//  for (commit in pullRequest['commits']) {
//    for (comment  in commit['comments']) {
//      echo "Commit: ${commit['sha']}, Author: ${comment['user']}, Body: ${comment['body']}"
//    }
//  }
  
//  for (comment in pullRequest['comments']) {
//      echo "Comment, Author: ${comment['user']}, Body: ${comment['body']}"    
//  }
    
//  for (reviewComment in pullRequest['review_comments']) {
//      echo "Review comment, Author: ${reviewComment['user']}, Body: ${reviewComment['body']}"    
//  }    
  
//  for (comment in pullRequest.comments) {
//    comment.delete()
//  }
  
//  pullRequest.createReviewRequests('aaronjwhiteside')
}
}
stage ('post-test') {
  
}
