# node-with-lerna-builder
Node.js 12.16 with Lerna installed

Sample _cloudbuild.yaml_
```
steps:
- name: 'roneru/node-with-lerna-builder'
  args: ['npm', 'install']
  waitFor: ['-']
  
- name: 'roneru/node-with-lerna-builder'
  args: ['lerna', 'bootstrap']
  waitFor: ['-']
```
