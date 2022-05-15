1. Had Problems running on gradle
2. Had to configure gradle JVM to Java 11
![](screenshots/0_gradle_config.png)

3. Ran Gumball Locally
![](screenshots/gumball.png)

4. Created CI Workflow
![](screenshots/1_gradle_yml.png)

5. Build Success
![](screenshots/2_build_success.png)

6. Generated Key
![](screenshots/3_generate_key.png)

7. Created GKE Secrets
![](screenshots/4_gke_secrets.png)

8. Release Made
![](screenshots/5_relesase.png)

9. Publish Release
![](screenshots/6_publish_release.png)

- I ran into a problem where the CD workflow was not executing after I published a release. I suspect it has something to do with GKE_PROJECT and GKE_SA_KEY secrets content I added.
- I tried referencing https://github.com/google-github-actions/setup-gcloud/blob/main/example-workflows/gke/README.md for help but no luck on getting the workflow to execute.
