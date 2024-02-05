# TestSemRelease


semantic-release "--no-ci" "--debug" "--dry-run"

npm install --save-dev semantic-release

npx semantic-release

npx semantic-release --no-ci --debug --dry-run > output.txt


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

set GITHUB_TOKEN=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
echo %GITHUB_TOKEN%


npm install --save-dev @semantic-release/commit-analyzer
npm install --save-dev @semantic-release/release-notes-generator
npm install --save-dev @semantic-release/changelog
npm install --save-dev @semantic-release/git

npm install --save-dev conventional-changelog-conventionalcommits
npm install @semantic-release/exec


npm install --no-save \
              semantic-release \
              @semantic-release/git \
              @semantic-release/changelog \
              @semantic-release/npm \
              @semantic-release/exec \
              @semantic-release/gitlab \
              conventional-changelog-conventionalcommits --legacy-peer-deps

branches: [
		'main',
		// version number branches will release that version
		'+([0-9])?(.{+([0-9]),x}).x',
		{
			channel: 'alpha',
			name: 'alpha/*',
			prerelease: true,
		},

----------------------------testing plan----------------------

main 
 


-------------------------bk-------------------------------
plugins:
    - path: "@semantic-release/commit-analyzer"
      preset: conventionalcommits
    - path: "@semantic-release/exec"
      analyzeCommitsCmd: ./.set-version.sh "${lastRelease.version}" "last"
      prepareCmd: ./.set-version.sh "${nextRelease.version}" "next"
    - "@semantic-release/release-notes-generator"
    - "@semantic-release/changelog"
    - path: "@semantic-release/git"
      message: "chore(release): ${nextRelease.version}\n\n${nextRelease.notes}"


{
  "repositoryUrl": "https://github.com/pashokchakravarthi/TestSemRelease.git",
  "branches": ["master", "main"]
}



main


