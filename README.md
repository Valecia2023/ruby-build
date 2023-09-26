# ruby-build
Compile and install - name: CodeQL Bundle
  # You may pin to the exact commit or the version.
  # uses: advanced-security/codeql-bundle-action@9437ba7f33c2a978c8897fb21b2a7e0809199d20
  uses: advanced-security/codeql-bundle-action@v1.1.0
  with:
    # The tag of bundle release to customize (e.g., codeql-bundle-20220311)
    bundle-version: # optional, default is latest
    # A comma-separated list of CodeQL packs to include in the bundle
    packs: 
    # Root directory where the codeql-workspace.yml file is located
    workspace: # optional, default is .
    # Upload the created bundle
    upload: # optional, default is true
    # 
    token: # optional, default is ${{ github.token }}
    # The max number of packs that will be processed concurrently
    concurrency-limit: # optional, default is 2
