
def podLabel = "worker-${UUID.randomUUID()}"

podTemplate(
  label: podLabel,
  containers: [
     containerTemplate(
       name: 'dotnet',
       image: 'microsoft/dotnet',
       ttyEnabled: true,
       command: 'cat')
     ]) {

     node(podLabel) {
       stage('test') {
         container('dotnet') {
           sh 'dotnet test demo'
         }
       }
     }
}
