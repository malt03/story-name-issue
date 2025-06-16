[Storybook](https://684fe690b6355c751bfefdd4-ylxeddyxrc.chromatic.com/)

```tsx
import type { Meta, StoryObj } from "@storybook/react-vite";

import { Foo } from "./Foo";

const meta = { component: Foo } satisfies Meta<typeof Foo>;

export default meta;
type Story = StoryObj<typeof meta>;

export const A: Story = {
  name: "NameA",
};

export const B: Story = {
  name: "NameB",
};

export const C: Story = {
  name: `NameC`,
};

export const D: Story = {
  name: "NameD" as const,
};

export const E: Story = {};
E.name = "NameE";
```
