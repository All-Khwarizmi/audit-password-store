### [S-#] The `PasswordStore::getPassword` function does not have any paramater whereas comments says it does which is confusing.

**Description:**
The `PasswordStore::getPassword` function signature is `function getPassword() external view returns (string memory)` but the natspec say it is `function getPassword(string memory newPassword) external view returns (string memory)`. This is confusing and can lead to confusion.

**Impact:**
The natspec is incorrect.

**Recommended Mitigation:**
Update the natspec to match the function signature.

```diff
-      * @param newPassword The new password to set.
```
