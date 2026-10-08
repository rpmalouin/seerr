# Fork Explanation and Support Standard

## Why This Fork Exists
This fork was created to implement critical security improvements that were missing in the upstream Seerr repository. Specifically, several administrative endpoints were lacking proper permission checks, allowing regular authenticated users to perform actions that should be restricted to administrators only.

## Our Standard: You Fork, You Support
We believe in the principle that if you fork a repository, you take on the responsibility of supporting that fork. This means:
- Keeping your fork up to date with upstream changes if you wish to stay current.
- Addressing any issues that arise in your fork.
- Being transparent about the differences between your fork and the upstream repository.
- Contributing back to upstream when possible, especially for bug fixes and improvements that benefit the broader community.

In the case of this fork, the security improvements are intended to be contributed back to the upstream Seerr project via a pull request. Until those changes are merged upstream, this fork provides a secure version of Seerr for users who require these protections immediately.

## How to Use This Fork
If you choose to use this fork, please:
1. Review the changes in `MEMORY.md` to understand what has been modified.
2. Monitor the upstream Seerr repository for updates and consider rebasing or merging those updates into this fork as needed.
3. If you encounter issues, first check if they are related to the changes made in this fork.
4. Consider contributing your improvements back to upstream Seerr.

## License
This fork maintains the same license as the upstream Seerr project (MIT License). See the [LICENSE](./LICENSE) file for details.