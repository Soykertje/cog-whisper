# Whisper Cog model

[![Replicate](https://replicate.com/openai/whisper/badge)](https://replicate.com/soykertje/whisper) 

This is an implementation of [Whisper](https://github.com/openai/whisper) as a Cog model using the latest available version
and adding more inputs in the predict function. [Cog packages machine learning models as standard containers.](https://github.com/replicate/cog)

First, run `get_weights.sh` from the project root to download pre-trained weights:

    ./scripts/get_weights.sh

You can then build a container and run predictions like so:

    cog predict -i audio="<path/to/your/audio/file>"

To publish the model to Replicate, run:

    cog login
    cog push r8.im/<your-username>/<your-model-name>

