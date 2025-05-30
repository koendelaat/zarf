---
title: zarf completion zsh
description: Zarf CLI command reference for <code>zarf completion zsh</code>.
tableOfContents: false
---

<!-- Page generated by Zarf; DO NOT EDIT -->

## zarf completion zsh

Generate the autocompletion script for zsh

### Synopsis

Generate the autocompletion script for the zsh shell.

If shell completion is not already enabled in your environment you will need
to enable it.  You can execute the following once:

	echo "autoload -U compinit; compinit" >> ~/.zshrc

To load completions in your current shell session:

	source <(zarf completion zsh)

To load completions for every new session, execute once:

#### Linux:

	zarf completion zsh > "${fpath[1]}/_zarf"

#### macOS:

	zarf completion zsh > $(brew --prefix)/share/zsh/site-functions/_zarf

You will need to start a new shell for this setup to take effect.


```
zarf completion zsh [flags]
```

### Options

```
  -h, --help              help for zsh
      --no-descriptions   disable completion descriptions
```

### Options inherited from parent commands

```
  -a, --architecture string        Architecture for OCI images and Zarf packages
      --insecure-skip-tls-verify   Skip checking server's certificate for validity. This flag should only be used if you have a specific reason and accept the reduced security posture.
      --log-format string          Select a logging format. Defaults to 'console'. Valid options are: 'console', 'json', 'dev'. (default "console")
  -l, --log-level string           Log level when running Zarf. Valid options are: warn, info, debug, trace (default "info")
      --no-color                   Disable terminal color codes in logging and stdout prints.
      --plain-http                 Force the connections over HTTP instead of HTTPS. This flag should only be used if you have a specific reason and accept the reduced security posture.
      --tmpdir string              Specify the temporary directory to use for intermediate files
      --zarf-cache string          Specify the location of the Zarf cache directory (default "~/.zarf-cache")
```

### SEE ALSO

* [zarf completion](/commands/zarf_completion/)	 - Generate the autocompletion script for the specified shell

