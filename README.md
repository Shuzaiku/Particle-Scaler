# Particle Scaler

--

## Introduction

Particle Scaler is a Roblox Studio plugin that enables dynamic scaling of ParticleEmitters over their lifetime and emit duration.

Particle Scaler is intended to work in pair with PrimeVoxel's VFX Suite plugin, as it mostly works as an extension of its "Emit" functionality.

Scaling is not meant to be a replacement of the ParticleEmitter's "Size" property, rather, it works in conjunction with it by evenly scaling the Size along the lifetime and duration of the particle emitter. Additionally, the "EmitDuration" attribute is taken into account when determining scaling, so it becomes possible for the particle emitter to be rescaled even when its performing continuous emission.

--

## Usage

#### ParticleEmitter Attributes

- EmitScale [NumberSequence]: The scale of the particle emitter at each keypoint.
  *Default: NumberSequence.new(0)*
  *Note: Due to Roblox limitations, NumberSequence can only range from 0 to 1, but
   the ScaleRange attribute can be used to override this range.*
	
- ScaleRange [NumberRange]: The minimum and maximum values that EmitScale can reach.
  *Default: NumberRange.new(0, 1)*


--

## Notes

- Scaling is subject to the same limitations as ParticleEmitter's "Size" property, so it is only capable of changing the size of particles within the range of 0 to 200.
- This plugin is not officially supported and it is not recommended for commercial use.
