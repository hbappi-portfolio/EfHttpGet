# EfHttpGet
a simple Http Request Client

# How to
To get a Git project into your build:

Step 1. Add the JitPack repository to your build file

gradle
maven
sbt
leiningen
Add it in your root build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
Step 2. Add the dependency

	dependencies {
		implementation 'com.github.User:Repo:[![](https://jitpack.io/v/hbappi/EfHttpGet.svg)](https://jitpack.io/#hbappi/EfHttpGet)'
	}
That's it! The first time you request a project JitPack checks out the code, builds it and serves the build artifacts (jar, aar).

If the project doesn't have any GitHub Releases you can use the short commit hash or 'master-SNAPSHOT' as the version.


now call
    
    EfHttpGet.stringResponse(url, new EfResponseListener() {
            @Override
            public void onSuccess(String response) {
	    	//you got server response as string. yahoo
            }

            @Override
            public void onError(String errorResponse) {
	    	//something wrong, error response is in string format
            }
        });

Youtube Video: https://www.youtube.com/watch?v=FAVWvT1RiYg

my linkedIn: https://www.linkedin.com/in/hbappi/
