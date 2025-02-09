# EpisodeData

## minari.EpisodeData

```{eval-rst}
.. autoclass:: minari.EpisodeData
```

### Attributes

```{eval-rst}
.. autoattribute:: minari.EpisodeData.id

    The ID of the episode in the Minari dataset.

.. autoattribute:: minari.EpisodeData.seed

    The seed used to reset this episode in the Gymnasium API.

.. autoattribute:: minari.EpisodeData.total_timesteps

    The number of timesteps contained in this episode.

.. autoattribute:: minari.EpisodeData.observations

    The observations of the environment. The initial and final observations are included meaning that the number
    of observations will be increased by one compared to the number of timesteps

.. autoattribute:: minari.EpisodeData.actions

    The actions taken in each episode timestep.

.. autoattribute:: minari.EpisodeData.terminations

    The ``terminated`` value after each environment step.

.. autoattribute:: minari.EpisodeData.truncations

    The ``truncated`` value after each environment step.
```
