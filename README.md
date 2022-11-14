# David

Hi Amaro. I got this to work with the following commands:

`brew tap AdoptOpenJDK/openjdk`
`brew install --cask adoptopenjdk8`

&

`pip install git+https://github.com/minerllabs/minerl`

But I can't any of the environments to load:

```bash
Traceback (most recent call last):
  File "/Users/dirk/.virtualenvs/David/lib/python3.10/site-packages/gym/envs/registration.py", line 150, in spec
    return self.env_specs[id]
KeyError: 'MineRLObtainDiamondVectorObf-v0'

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "/Users/dirk/Documents/David/minerl.py", line 2, in <module>
    import minerl
  File "/Users/dirk/Documents/David/minerl.py", line 8, in <module>
    env = gym.make('MineRLObtainDiamondVectorObf-v0')
  File "/Users/dirk/.virtualenvs/David/lib/python3.10/site-packages/gym/envs/registration.py", line 184, in make
    return registry.make(id, **kwargs)
  File "/Users/dirk/.virtualenvs/David/lib/python3.10/site-packages/gym/envs/registration.py", line 105, in make
    spec = self.spec(path)
  File "/Users/dirk/.virtualenvs/David/lib/python3.10/site-packages/gym/envs/registration.py", line 167, in spec
    raise error.UnregisteredEnv("No registered env with id: {}".format(id))
gym.error.UnregisteredEnv: No registered env with id: MineRLObtainDiamondVectorObf-v0
```