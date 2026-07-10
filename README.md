local llm setup with docker sandbox + lm studio + pi + qwen 

model - qwen/qwen3.6-35b-a3b

model - qwen2.5-coder-3b

start docker sandbox and use ai agent pi with local llm qwen3.6 

---

open terminal pwsh


check existing docker sandbox with :

	sbx or sbx ls


if none :

then to make a new docker sandbox with pi as agent with all the skills setup from my GitHub run : 

	sbx run pi --kit "git+https://github.com/ArifAziz99/docker-sandbox.git#dir=pi" --kit "git+https://github.com/ArifAziz99/docker-sandbox.git#dir=skills"


if exists :

then to get back into sandbox run :

	sbx exec -it pi-AI /bin/bash

note: instead of pi-AI add your sandbox name shown with sbx ls


then inside the sandbox to start/continue pi run : 

	pi -c



then in another terminal load a model from lm studio run :

	lms load

note: start lmstudio server from it gui(app) if not already
