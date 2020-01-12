
## Default Variables

### ruby_global_gems

List of gems to install system-wide

#### Default value

```yaml
ruby_global_gems: []
```

#### Example usage

```yaml
ruby_user_gems:
  - gemname1
  - name: gemname1
    verison: 1.0.0
    pre_release: False
    state: latest
```

### ruby_install

Install ruby via homebrew

#### Default value

```yaml
ruby_install: false
```

### ruby_user

User to run user-specific commands

#### Default value

```yaml
ruby_user | default(homebrew_user) | default(ansible_user_id)
```

### ruby_user_gems

List of gems to install for an user

#### Default value

```yaml
ruby_user_gems: []
```

#### Example usage

```yaml
ruby_user_gems:
  - gemname1
  - name: gemname1
    verison: 1.0.0
    pre_release: False
    state: latest
```
## Dependencies

None

## License

Apache-2.0

## Author

Thomas Boerger
